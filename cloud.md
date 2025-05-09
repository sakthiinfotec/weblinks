#### MicroVMs
- Flintlock: handles the interaction with the microvm implementation (i.e. Firecracker, Cloud Hypervisor)
- [Firecracker: Secure and fast microVMs for serverless computing. Firecracker is an open source virtualization technology that is purpose-built for creating and managing secure, multi-tenant container and function-based services.](https://firecracker-microvm.github.io/)
- [Cloud Hypervisor: Run Cloud Virtual Machines Securely and Efficiently](https://www.cloudhypervisor.org/)
 
#### Object storages
- Azure Blob Storage
- AWS S3
- Google Cloud Storage

#### Pulumi
* [How do you make an s3 bucket with a lifecycle policy?](https://www.pulumi.com/ai/conversations/f925073d-2997-4aaf-ae16-177931a31474)
* [How to set a 1-week expiration on S3 bucket objects?](https://www.pulumi.com/ai/answers/bkxFpzbdFirqc1R5UKdmjw/setting-1-week-expiration-on-aws-s3-objects)
* [Automating AWS S3 bucket policies and lifecycle rules with Travis CI with Terraform](https://www.pulumi.com/ai/answers/5926pfa21VUbymMsAPbC76/automating-aws-s3-policies-with-terraform-and-travis-ci)
* [GCP AutoML Vision image classification with Terraform](https://www.pulumi.com/ai/conversations/25492f9b-9d3f-47e0-b1e1-cd1085db1e42)  

[temporal.io - The Open Source Runtime for Go/Java/Node.js service orchestration at scale](https://temporal.io/)  
[Event-Driven Orchestration: Effective Microservices Integration Using BPMN and AMQP](https://dzone.com/articles/event-driven-orchestration-an-effective-microservi)  

##### Certification
[TechGig - Cloud DevJam](https://www.techgig.com/googlecloud)  
[AWS Certified Solutions Architect Associate SAA-C03 Video Course - Tutorials Dojo](https://portal.tutorialsdojo.com/courses/aws-certified-solutions-architect-associate-exam-video-course/)  

##### Cloud Deployments
- [Python Anywhere - Deploy Python Web app on the Cloud!](https://www.pythonanywhere.com/)  
- [Heroku - Deploy Python, Node.js, Ruby, Go and Java applications!](https://www.heroku.com/)  
- [Depot - Accelerate your Docker image builds and GitHub Actions workflows.](https://depot.dev/)
- [Open Status - Status Monitoring Services](https://www.openstatus.dev/)
- [Runway ML - Generative AI Audio, Video, Text-to-Image | Text-to-Video | Image-to-Video](https://runwayml.com/)
- [Scaleway - Europe based Cloud Provider. Build, train, deploy and scale AI models and intelligent applications on a resilient and sustainable cloud ecosystem.](https://www.scaleway.com/en/)
- [Fly.io: Deploy app server close to your users | A Public Cloud Built For Developers Who Ship](https://fly.io/)
- [Render: Cloud Application Platform](https://render.com/)
- [Vercel: Build and deploy the best web experiences with the Frontend Cloud](https://vercel.com/)
- [Utho: Cloud Service Provider India](https://utho.com)
- [OVHcloud India: Cloud Computing & Web Hosting](https://www.ovhcloud.com/en-in/)
- [TiDB: The Distributed SQL Database by PingCAP. TiDB delivers resilient performance, real-time insights, secure and flexible data infrastructure at any scale.](https://www.pingcap.com/)
- [Vultr: SSD VPS Servers, Cloud Servers and Cloud Hosting. Global, automated cloud infrastructure from the broadest array of AMD and NVIDIA GPUs to virtual CPUs, bare metal, Kubernetes, storage, and networking solutions.](https://www.vultr.com/)
- [Qovery is a DevOps Automation Platform](https://www.qovery.com/)
- [Flightcontrol is a PaaS that deploys to your AWS account](https://www.flightcontrol.dev/)
- [Appfleet: appfleet is an edge platform | A simple Kubernetes alternative Edge docker hosting made simple.](https://appfleet.com/)
- [Apache CloudStack™ is an open-source software system designed to deploy and manage large networks of virtual machines, as a highly available, highly scalable Infrastructure as a Service (IaaS) cloud computing platform.](https://cloudstack.apache.org/)
- [OpenNebula: The Open Source Cloud & Edge Computing Platform](https://opennebula.io/)
- [Plural: Enterprise Kubernetes management, accelerated | DevOps, K8s,](https://www.plural.sh/)
- [Bunnyshell environments are built to Test, Review & Deploy AI-Generated code at Lightspeed!](https://www.bunnyshell.com/)
- [Gitpod.io: Automated, standardized, and secure development environments](https://www.gitpod.io/)
- [Coder: Secure environments for developers and their agents | Self-Hosted Cloud Development Environment](https://coder.com/)

#### Workflow / Orchestration
- [Inngest: AI and backend workflows, orchestrated at any scale](https://www.inngest.com/)
- [Windmill: Open-source developer platform and workflow engine](https://www.windmill.dev/)

#### Cloud Services
- Infrastructure as Code (IaC):
   * Terraform
   * AWS CloudFormation (AWS)
   * Azure Resource Manager templates (Azure)
   * Deployment Manager (GCP) 
- Manage Organizations / Projects / Groups
  * IAM Users and Roles: AWS Organizations for managing multiple accounts which can be useful if the client has multiple AWS accounts
  * Service Accounts and IAM: Use GCP's IAM to manage access. GCP Projects can also help in organizing resources where you can be granted access to individual projects instead of the whole account
  * Azure Active Directory (Azure AD) and Role-Based Access Control (RBAC): Use Azure AD for identity management and RBAC for defining permissions. Azure has a concept of Management Groups and Subscriptions which can be used to delegate control.
- Cloud Shell: Each provider offers a cloud-hosted shell environment where you can run scripts and manage resources directly from the browser:
  * AWS CloudShell
  * Azure Cloud Shell
  * Google Cloud Shell
- Audit logs
   * AWS CloudTrail
   * Azure Monitor Logs
   * GCP Cloud Audit Logs

#### Best Practices
- [Cloudian - Understanding AWS S3 Storage Pricing: A Comprehensive Guide](https://cloudian.com/blog/5-components-of-aws-s3-storage-pricing/)
- [CloudZero - The No BS Guide To Understanding S3 Storage Costs](https://www.cloudzero.com/blog/s3-pricing/)  
