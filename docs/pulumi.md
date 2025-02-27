### 1. I want a static website on AWS behind a CloudFront CDN, or I want an Ubuntu Linux server that I can access over SSH.
Let's create a static website on AWS behind a CloudFront CDN. This involves creating an S3 bucket to host the website, setting up the bucket policy, and configuring CloudFront to serve the content from the S3 bucket.

Here's a Pulumi program in TypeScript to achieve this:
```TypeScript
import * as pulumi from "@pulumi/pulumi";
import * as aws from "@pulumi/aws";

// Create an S3 bucket to host the static website
const siteBucket = new aws.s3.Bucket("siteBucket", {
    website: {
        indexDocument: "index.html",
        errorDocument: "error.html",
    },
});

// Upload the index.html and error.html files to the bucket
const indexHtml = new aws.s3.BucketObject("index.html", {
    bucket: siteBucket,
    source: new pulumi.asset.FileAsset("index.html"), // Make sure you have this file locally
    contentType: "text/html",
});

const errorHtml = new aws.s3.BucketObject("error.html", {
    bucket: siteBucket,
    source: new pulumi.asset.FileAsset("error.html"), // Make sure you have this file locally
    contentType: "text/html",
});

// Set the bucket policy to allow public read access
const bucketPolicy = new aws.s3.BucketPolicy("bucketPolicy", {
    bucket: siteBucket.bucket,
    policy: siteBucket.bucket.apply(publicReadPolicyForBucket),
});

function publicReadPolicyForBucket(bucketName: string): string {
    return JSON.stringify({
        Version: "2012-10-17",
        Statement: [{
            Effect: "Allow",
            Principal: "*",
            Action: ["s3:GetObject"],
            Resource: [`arn:aws:s3:::${bucketName}/*`],
        }],
    });
}

// Create a CloudFront distribution to serve the content from the S3 bucket
const cdn = new aws.cloudfront.Distribution("cdn", {
    origins: [{
        domainName: siteBucket.websiteEndpoint,
        originId: siteBucket.arn,
    }],
    enabled: true,
    isIpv6Enabled: true,
    defaultRootObject: "index.html",
    defaultCacheBehavior: {
        allowedMethods: ["GET", "HEAD"],
        cachedMethods: ["GET", "HEAD"],
        targetOriginId: siteBucket.arn,
        forwardedValues: {
            queryString: false,
            cookies: { forward: "none" },
        },
        viewerProtocolPolicy: "redirect-to-https",
        minTtl: 0,
        defaultTtl: 3600,
        maxTtl: 86400,
    },
    priceClass: "PriceClass_100",
    restrictions: {
        geoRestriction: {
            restrictionType: "none",
        },
    },
    viewerCertificate: {
        cloudfrontDefaultCertificate: true,
    },
});

// Export the URLs
export const bucketName = siteBucket.bucket;
export const cdnUrl = cdn.domainName;
```
This program creates an S3 bucket configured to host a static website, uploads index.html and error.html files to the bucket, sets the bucket policy to allow public read access, and creates a CloudFront distribution to serve the content from the S3 bucket. The URLs for the bucket and the CloudFront distribution are exported as stack outputs.

### 2. I want to setup an Kubernetes infrastructure for my e-commerce services with following stack (Kafka, PostgreSQL, Redis) React Web in CDN along with with following Microservices (in Nest.JS) 1. Order Service 2. Customer Service 3. Inventory Service 4. Notification Service 5. Payment Service

To set up a Kubernetes infrastructure for your e-commerce services with the specified stack, we will use Pulumi to create a Kubernetes cluster and deploy the necessary services. We will also set up a CDN for your React web application. Here is a Pulumi program to achieve this:

Create a Kubernetes cluster.
Deploy Kafka, PostgreSQL, and Redis.
Deploy the React web application in a CDN.
Deploy the microservices (Order, Customer, Inventory, Notification, and Payment) in Nest.JS.
```TypeScript
import * as pulumi from "@pulumi/pulumi";
import * as k8s from "@pulumi/kubernetes";
import * as aws from "@pulumi/aws";
import * as awsx from "@pulumi/awsx";
import * as cloudflare from "@pulumi/cloudflare";

// Create a VPC for the Kubernetes cluster
const vpc = new awsx.ec2.Vpc("ecommerce-vpc", {
    numberOfAvailabilityZones: 2,
});

// Create an EKS cluster
const cluster = new awsx.eks.Cluster("ecommerce-cluster", {
    vpcId: vpc.id,
    subnetIds: vpc.publicSubnetIds,
    instanceType: "t3.medium",
    desiredCapacity: 2,
});

// Export the cluster's kubeconfig
export const kubeconfig = cluster.kubeconfig;

// Deploy Kafka
const kafka = new k8s.helm.v3.Chart("kafka", {
    chart: "kafka",
    version: "12.0.1",
    fetchOpts: { repo: "https://charts.bitnami.com/bitnami" },
}, { provider: cluster.provider });

// Deploy PostgreSQL
const postgresql = new k8s.helm.v3.Chart("postgresql", {
    chart: "postgresql",
    version: "10.3.14",
    fetchOpts: { repo: "https://charts.bitnami.com/bitnami" },
}, { provider: cluster.provider });

// Deploy Redis
const redis = new k8s.helm.v3.Chart("redis", {
    chart: "redis",
    version: "14.8.8",
    fetchOpts: { repo: "https://charts.bitnami.com/bitnami" },
}, { provider: cluster.provider });

// Deploy React web application to a CDN
const bucket = new aws.s3.Bucket("react-web-bucket", {
    website: {
        indexDocument: "index.html",
    },
});

const cdn = new cloudflare.Record("react-web-cdn", {
    zoneId: "your-cloudflare-zone-id",
    name: "www",
    type: "CNAME",
    value: bucket.websiteEndpoint,
});

const bucketObject = new aws.s3.BucketObject("index.html", {
    bucket: bucket,
    source: new pulumi.asset.FileAsset("path-to-your-react-app-build/index.html"),
    acl: "public-read",
    contentType: "text/html",
});

// Deploy Nest.JS microservices
const services = ["order", "customer", "inventory", "notification", "payment"];

services.forEach(service => {
    const appLabels = { app: service };
    const deployment = new k8s.apps.v1.Deployment(`${service}-deployment`, {
        metadata: { name: service },
        spec: {
            replicas: 2,
            selector: { matchLabels: appLabels },
            template: {
                metadata: { labels: appLabels },
                spec: {
                    containers: [{
                        name: service,
                        image: `your-docker-repo/${service}:latest`,
                        ports: [{ containerPort: 3000 }],
                    }],
                },
            },
        },
    }, { provider: cluster.provider });

    const serviceResource = new k8s.core.v1.Service(`${service}-service`, {
        metadata: { name: service },
        spec: {
            type: "LoadBalancer",
            selector: appLabels,
            ports: [{ port: 80, targetPort: 3000 }],
        },
    }, { provider: cluster.provider });
});

export const cdnUrl = cdn.name;
```
This program sets up the following:

1. A Kubernetes cluster on AWS using EKS.
2. Deploys Kafka, PostgreSQL, and Redis using Helm charts.
3. Sets up an S3 bucket for your React web application and configures a Cloudflare CDN.
4. Deploys the Nest.JS microservices for Order, Customer, Inventory, Notification, and Payment services.

Make sure to replace "your-cloudflare-zone-id", "path-to-your-react-app-build/index.html", and "your-docker-repo" with your actual Cloudflare zone ID, the path to your React app build, and your Docker repository respectively.
