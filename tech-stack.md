### Technology Stacks

##### Design
[Spline - 3D Design in Web Browser](https://spline.design/)  
[Rive - Design and Animation app for Mobile and Web](https://rive.app)  

##### Authentication & Authorization
- SSO tokens
- OAuth 2.0 and JWT patterns

##### Frameworks: 
- React 
- NextJS 
- Storybook
- Micro Front End

##### State Management
- [Zustand](https://github.com/pmndrs/zustand)
- [Redux](https://redux.js.org/)

##### REST API
- [Learn REST: A RESTful Tutorial](https://www.restapitutorial.com/)  
- [REST CookBook](https://restcookbook.com/)  
- [Service Architecture - Representational State Transfer (REST) | RDBMS | ORM | Cloud Computing](https://www.service-architecture.com/articles/web-services/representational-state-transfer-rest.html)  

##### Schema Validation
- [Zod - TypeScript-first schema validation with static type inference](https://github.com/colinhacks/zod)  
- [Yup - Dead simple Object schema validation](https://github.com/jquense/yup)  
- [Superstruct - A simple and composable way to validate data in JavaScript (and TypeScript).](https://github.com/ianstormtaylor/superstruct)  

##### Datastores
- [DuckDB](https://github.com/duckdb/duckdb): is a in-process and high-performance analytical(OLAP) database system.  
- [PocketBase - an open source realtime Go backend in 1 file](https://github.com/pocketbase/pocketbase)  
[DuckDB - Introduction to DuckDB and its Python integration](https://towardsdatascience.com/forget-about-sqlite-use-duckdb-instead-and-thank-me-later-df76ee9bb777)  
[Run PostgreSQL - Cloud Native way](https://cloudnative-pg.io/)  
[SQLBolt - Learn SQL with simple, interactive excercises](https://sqlbolt.com/)  
[Xata.io(PostgreSQL + Elasticsearch) - The serverless database that gives you superpowers | 15GB Free | RDBMS | Search Engine | Vector DB | Edge Caching | Production Ready](https://xata.io/)  

##### Vector Databases

- Pinecone
- Weaviate
- Chroma
- Qdrant
- Typesense - used to build blazing-fast search experiences, faceted navigation experiences, geo-search, vector search, semantic search, similarity search and much more.

##### Headless CMS
- Contentful
- Strapi
- Dato CMS
- Prismic

##### Data Formats
- [MessagePack](https://msgpack.org/) - It's like JSON but fast and small. MessagePack is an efficient binary serialization format. It lets you exchange data among multiple languages like JSON. But it's faster and smaller. Small integers are encoded into a single byte, and typical short strings require only one extra byte in addition to the strings themselves. 

##### Microservices
- [Envoy is an open source edge and service proxy, designed for cloud-native applications](https://www.envoyproxy.io/)  
- [Envoy Mobile](https://envoymobile.io/)  
- [Istio - Simplify observability, traffic management, security, and policy with the leading service mesh](https://istio.io/latest/)  

##### Microservices - Communication
Typically external application clients such as web apps, mobile apps or IoT frameworks consume RESTfull API endpoints. However, modern backend developers usually don’t call microservices directly because of scaling problems and network security issues. Therefore, before exposing your microservices to the internet, developers will connect them to an API gateway or load balancer.

While inter-service communication happens via
- Synchronous - REST API, gRPC
- Asynchronous - Message based using message brokers like RabbitMQ

**Messaging patterns:** RPC, MPI, pub/sub, CQRS

##### Microservices - Tracers
- [Zipkin](https://zipkin.io/)  
- [Jaeger - Distributed Tracing Platform](https://github.com/jaegertracing/)  
- [DataDog - Modern monitoring & security](https://datadoghq.com/)  
- [Apache - SkyWalking: Application performance monitor tool for distributed systems, especially designed for microservices, cloud native and container-based (Kubernetes) architectures](https://skywalking.apache.org/)  
- [Prometheus - Prometheus - Monitoring system & time series database](https://prometheus.io/)  
- Observability (with Grafana and Prometheus)
- Traceability (with Kiali and Jaeger)
- Canary Deployments & Rolling Updates (with Istio)
- API routing & Management (with Istio )
- OpenShift ServiceMesh
- [Fluent Bit - An End to End Observability Pipeline](https://fluentbit.io/how-it-works/)  
- [OpenTelemetry - High-quality, ubiquitous, and portable telemetry to enable effective observability](https://opentelemetry.io/)  

##### Data Science
- [JupyterLab - Docs](https://jupyterlab.readthedocs.io/en/stable/index.html)  
- [Developing JupyterLab Extensions](https://tech.target.com/blog/developing-jupyterlab-extensions)  
- [Gradio - Build & Share Delightful Machine Learning Apps](https://gradio.app/)  
- [Streamlit - A faster way to build and share data apps](https://streamlit.io/)  
- [Dash - Build data apps in Dash | Dash is the leading low-code platform for data apps](https://plotly.com/dash/)  

##### AI/ML
- NLU
  - [DeepPavlov - an open-source conversational AI library built on PyTorch](https://github.com/deeppavlov/DeepPavlov)  
  - [Rasa is an open source machine learning framework to automate text and voice-based conversations](https://github.com/RasaHQ/rasa)  
- [Featuretools - An open source python library for automated feature engineering](https://www.featuretools.com/)  

##### MLOps
- [Machine Learning Operations @ ml-ops.org](https://ml-ops.org/)  
- [Machine Learning Workflow - Streamlining Your ML Pipeline @ run.ai](https://www.run.ai/guides/machine-learning-engineering/machine-learning-workflow)  

##### Serverless
[AWS Chalice - A framework for writing serverless applications](https://aws.github.io/chalice/)  

##### Containers: 
- Docker
- K8S

##### API Gateways
- [Kong](https://konghq.com/)  
- [Tyk](https://tyk.io/)  
- [Apigee](https://cloud.google.com/apigee)  

##### Rate Limit
[Set up rate limiting in Next.js with Redis](https://blog.logrocket.com/set-up-rate-limiting-next-js-redis/)  
[Rate Limiting Algorithms](https://www.npmjs.com/package/@upstash/ratelimit):  
- Fixed Window
- Sliding Window
- Token Bucket

##### CI
- Jenkins
- CircleCI

##### CD
- ArgoCD
- [Terraform](https://developer.hashicorp.com/terraform)  
- [Nomad](https://developer.hashicorp.com/nomad)  
- [Pulumi](https://www.pulumi.com/)  

##### Deployment
- Terraform
- [Render](https://render.com/) - Render is a unified cloud to build and run all your apps and websites with free TLS certificates, a global CDN, DDoS protection, private networks, and auto deploys from Git.
- Blue / Green Deployment

##### Monitoring
- Prometheus, Grafana
- AirBrake(Ruby) Alernatives: Rollbar, Scout, Sentry, Jira, LogRocket, Datadog, Wrike, ClickUp, monday.com, TrackJs, RayGun, HoneyBadger

##### Tooling: 
- npm, turborepo, webpack, babel, code-splitting
- [Rclone ("rsync for cloud storage") is a command-line program to sync files and directories to and from different cloud storage providers.](https://github.com/rclone/rclone)  
- [s5cmd - Parallel S3 and local filesystem execution tool](https://github.com/peak/s5cmd)  
- [SWC (Speedy Web Compiler) is a super-fast TypeScript / JavaScript compiler written in Rust.](https://github.com/swc-project/swc)  
- [Vite - Next generation front-end tooling. It's fast!](https://github.com/vitejs/vite)  
- [CodeMirror](https://codemirror.net/) - CodeMirror is a code editor component for the web.
- [terser](https://terser.org/) 
    * JavaScript mangler and compressor toolkit for ES6+
    * Terser is an industry-standard minifier for JavaScript code.
    * It removes comments, makes variable names smaller, and removes whitespace.
    * Readable and maintainable code patterns are replaced with smaller code.
    * Some variable references and function calls can be inlined into the places they're used.

##### Bundlers
- [Rspack - A fast Rust-based web bundler](https://github.com/web-infra-dev/rspack)  
- Pnpm
- [Turbopack - is an incremental bundler optimized for JavaScript and TypeScript, written in Rust, and built into Next.js](https://turbo.build/pack)  

##### Realtime DB / Notification
- Websocket
  - [Socket.io](https://ably.com/topic/socketio)  
  - [Socket.io v4](https://socket.io/docs/v4/)  
- Firebase
- [RethinkDB](https://rethinkdb.com/docs/quickstart)  
- [Liveblocks - The all-in-one toolkit to build collaborative products like Figma, Notion,](https://github.com/liveblocks/liveblocks)  
- Pusher
- [Conflict-Free Replicated Data Types as a way to sync data across devices](https://talk.objc.io/episodes/S01E294-crdts-introduction?t=6)  

##### Alert & Notifications
- [MailHog - Web and API based SMTP testing - written in Go](https://github.com/mailhog/MailHog)  
- [Sendgrid](https://sendgrid.com/)  
- [Postmark](https://postmarkapp.com/)  
- [Mailgun](https://www.mailgun.com/)  
- [SparkPost](https://www.sparkpost.com/)  
- [Sendwithus](https://www.sendwithus.com/)  
- [Email as a Microservice](https://www.cloudbees.com/blog/email-as-a-microservice)  
- [Open Source Live Chat](https://www.google.com/search?q=open+source+live+chat)  
- [Chatwoot](https://www.chatwoot.com/)  
- [LiveHelperChat](https://livehelperchat.com/)  
- [Chaskiq](https://www.chaskiq.io/)  
- [Helpy.io](https://helpy.io/live-chat/)  

##### Mobile
- React
  - [React Native UI Lib - is a UI Toolset & Components Library for React Native](https://wix.github.io/react-native-ui-lib/)  
  - [TamaGUI - Universal UI kit and style system for React Native + Web - with an optimizing compiler](https://github.com/tamagui/tamagui)  

##### Testing
- E2E: Selenium, Jest, Cypress, Playwright
- Integration: Snapshot
- Unit: Jest, Enzyme
- [Playwright - Enables reliable end-to-end testing for modern web apps](https://playwright.dev/)  
- [K6 - A modern load testing tool, using Go and JavaScript](https://k6.io/)  
- [Vitest - Blazing Fast Unit Test Framework](https://vitest.dev/)  
- [TestСafe - Cross-Browser End-to-End Testing Framework](https://testcafe.io/)  
- [Boilerplate for Playwright-Typescript framework for Web-UI, api, Mobile Emulation, DB and Visual testing](https://github.com/akshayp7/playwright-typescript-playwright-test)
- [Boilerplate for Playwright with Cucumber Java and JUnit](https://github.com/akshayp7/playwright-java-cucumber)  
- [Achieve integration testing without a UI in a way that is headless | the Pivot framework](https://dev.to/andyjessop/writing-integration-tests-that-run-inside-a-unit-testing-framework-like-jest-48f8)  

##### Media Servers
- Emby
- Jellyfin
- Jitsi
- Janus

##### Android
- Keep up to date with the latest best practices, common frameworks and tools to continuously define into a common set of coding guidelines and best practices for the app
- Have a deep understanding of modern Android development.
- Write readable, maintainable, performant and testable code.
- Kotlin, Coroutines, Flows, and the Android lifecycle, Compose

##### iOS
- Have a deep understanding of modern iOS development. 
- Comfortable with Swift and Objective C, iOS development fundamental, UIKit, AutoLayout, and Foundation

##### SDLC Concepts
- Deployment pipelines, Observability & Monitoring, Quality Assurance, Automation, Self-service
- Monorepo
- DORA metrics
- Infrastructure-as-code and configuration management
- Developer Experience and Platform Engineering
- Cloud Service Providers - Google Cloud Platform, Azure or AWS
- ArgoCD, CircleCI, Grafana, Prometheus, Kubernetes, GCP, Infrastructure as Code (Terraform), Service Mesh (Linkerd), Cloudflare

##### Documentation
[Jupyter Book - Build beautiful, publication-quality books and documents from computational content](https://jupyterbook.org/en/stable/start/build.html)  

##### Community Forum
[Discourse - Community Forum](https://github.com/discourse/discourse)  

##### How-to Guides
[Kubernetes MERN Stack Voting App](https://www.pulumi.com/registry/packages/aws/how-to-guides/aws-ts-k8s-mern-voting-app/)  
[Fullstack Pulumi: Deploying the MERN Stack on DigitalOcean](https://www.pulumi.com/blog/fullstack-pulumi-mern-stack-digitalocean/)  
[Deploying a Data Warehouse with Pulumi and Amazon Redshift](https://www.pulumi.com/blog/building-a-data-warehouse-on-aws-with-redshift-and-pulumi/)  
[Platform Engineering with Pulumi- Episode 1: Building the AWS Landing Zone with Pulumi](https://aws.plainenglish.io/platform-engineering-with-pulumi-episode-1-building-the-aws-landing-zone-with-pulumi-67b559523c78)  
[Platform Engineering with Pulumi Episode 2: Build and Deploy a React.js Application](https://aws.plainenglish.io/platform-engineering-with-pulumi-episode-2-building-and-deploying-the-nodejs-application-6217ed039e6)  
[Full Stack Application with Kubernetes, Quarkus, and React](https://abvijaykumar.medium.com/list/full-stack-application-with-kubernetes-quarkus-and-react-8707fcb7b717)  
[Why will I choose Pulumi over Terraform for my next project?](https://www.techwatching.dev/posts/pulumi-vs-terraform)  

##### For Startups
How to Start Online Earning with $0 Investment
- Brand ➔ Twitter is free
- Design ➔ Canva is free
- Website ➔ Carrd is free
- Store ➔ Gumroad is free
- Workspace ➔ Notion is free

##### Courses
10 FREE courses  
[1. Introduction to Computer Science 101](https://online.stanford.edu/courses/soe-ycscs101-computer-science-101)  
[2. Machine Learning Specialization](https://www.coursera.org/specializations/machine-learning-introduction)  
[3. Designing Your Career](https://online.stanford.edu/courses/tds-y0003-designing-your-career)  
[4. Introduction to Internet of Things](https://online.stanford.edu/courses/xee100-introduction-internet-things)  
[5. Databases: Advanced Topics in SQL](https://online.stanford.edu/courses/soe-ydatabases0001-databases-advanced-topics-sql)  
[6. Introduction to Game Theory](https://online.stanford.edu/courses/soe-ycs0002-game-theory)  
[7. R Programming Fundamentals](https://online.stanford.edu/courses/xfds112-r-programming-fundamentals)  
[8. Introduction to Cryptography](https://online.stanford.edu/courses/xfds112-r-programming-fundamentals)  
[9. Advanced Cybersecurity Program](https://online.stanford.edu/courses/xacs100-advanced-cybersecurity-program-preview)  
[10. Algorithms: Design and Analysis](https://online.stanford.edu/courses/soe-ycsalgorithms1-algorithms-design-and-analysis-part-1)  
[edX - Caltech - Learning From Data (Introductory Machine Learning)](https://www.edx.org/course/learning-from-data-introductory-machine-learning#!)  

##### [Tractable](https://tractable.ai/) - Tractable develops artificial intelligence for accident & disaster recovery.
- Python
- Node.js with Typescript 
- React for frontend development
- PostgreSQL for persistent data storage
- Kafka for asynchronous message queue
- Kubernetes and Docker to schedule and run services
- Jenkins to run testing and deployment pipelines
- AWS for infrastructure

##### [Tech stack of Navattic](https://jobs.polymer.co/navattic/27232)
- Typescript
- Next.js / Vercel
- PlanetScale
- GraphQL
- Prisma
- Cloudflare workers

##### [Intenseye](https://www.intenseye.com) - Intenseye is an AI-powered employee health and safety software platform
- Scala, Go, Python for programming languages.
- Google Cloud Platform (GCP) and Amazon Web Services (AWS) for cloud services.
- Docker, Kubernetes for orchestration tools.
- Apache Pulsar for message queueing.
- Prometheus, Grafana for monitoring. 
- Elasticsearch for analytics
- Redis for distributed caching.
- Linkerd for service mesh.
- Buildkite for CI/CD.
- PostgreSQL for RDBMS.
- Git for version control.
- Replicated for on-premise.

##### [IMMO](https://angel.co/company/immo-3/jobs/2335014-senior-software-engineer-backend)  - Real Estate Investment
- Node.js
- Serverless Framework
- PostgreSQL
- Python
- Airflow
- AWS
- Terraform
- Docker
- CircleCI
- GitHub

##### [Scaler](https://www.scaler.com/careers/staff-software-engineer-frontend) - Scaler Academy
High level of fluency and experience in technologies like  
a. HTML5, CSS3(BEM preferred), CSS Preprocessors (Sass/Less/PostCSS)  
b. Javascript ES6 & Typescript  
c. Frameworks (React with Redux/Mobx)  
d. Server-side Rendering (using Next.js)  
e. Static Stire Generators (Next.js/GatsbyJS)  
f. Build tools (Webpack/Esbuild)  
g. Package Managers (npm, yarn)  
h. Testing tools (Jest/Cypress/Enzyme)  
i. Linters (ESLint)  
j. Performance and Optimizations (AMP, Web Vitals & SEO Optimizations, Lighthouse, Dev Tools, PRPL/RAIL models, and Performance Metrics)  
k. Web development concepts like Web Security Fundamentals, CORS, Content Security Policies, Virtual DOM, Browser Storage, Web Sockets, Service Workers.  
