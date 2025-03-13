#### Microservices

![Microservices](./microservices.jpeg)

Companies like Netflix, Amazon, and others have adopted the concept of microservices in their products due to large benefits offered by microservices.

As we understand, many developers want to know how they should start this journey. So I decided to make this journey clearer by defining a road map for this learning curve.

**Container** - A container is a standard unit of software that packages up code and all its dependencies so the application runs quickly and reliably from one computing environment to another.

**Container orchestration** automates containers' deployment, management, scaling, and networking. Enterprises that need to deploy and manage hundreds or thousands of Linux® containers and hosts can benefit from container orchestration.

**Load balancer** is a device that acts as a reverse proxy and distributes network or application traffic across several servers.
Load balancers are used to increase the capacity (concurrent users) and reliability of applications. 
 
**Monitoring and Alerting**: In a microservice architecture, if you want to have a reliable application or service, you have to monitor the functionality, performance, communication, and any other aspect of your application in order to achieve a responsible application. Promethous is widely popular.

**Distributed Tracing** - when it comes to microservice architecture, a request may be passed through different services, which makes it difficult to debug and trace because the codebase is not in one place, so here distributed tracing tool can be helpful.

**Message Broker** - A message broker is software that facilitates the exchange of messages between applications, systems, and services.

**Database** - in most systems, we need to persist data, because we would need the data for further processes or reporting, etc.

**Caching** - Caching reduces latency in service-to-service communication of microservice architectures.

**Cloud service provider** - is a third-party company offering a cloud-based platform, infrastructure, application, or storage services.

**API Management**: API management is the process of designing, publishing, documenting, and analyzing APIs in a secure environment. 

**Application Gateway** - An application gateway or application level gateway (ALG) is a firewall proxy that provides network security. It filters incoming node traffic to certain specifications, meaning only transmitted network application data is filtered.

**Service Registration** - A service registry is a database used to keep track of the available instances of each microservice in an application. The service registry needs to be updated each time a new service comes online and whenever a service is taken offline or becomes unavailable.

Credits to [LinkedIn Post](https://www.linkedin.com/feed/update/urn:li:activity:7008442011582107648?utm_source=share&utm_medium=member_desktop)   

**Load balancer algorithms:**
- Load balancers can route traffic based on various metrics like least-busy, random, round-robin, sticky, etc.

#### [How to Design a Chat Application like WhatsApp](https://x.com/ashishps_1/status/1889532829853524125)
🔹 Chat Servers - Manages a large number of concurrent WebSocket connections, facilitate real-time communication, and ensure that messages are delivered efficiently between users with minimal latency.

🔹 Load Balancer - Distributes traffic across multiple chat server instances. Uses sticky sessions to ensure clients consistently connect to the same server.

🔹 User Connection Cache - A fast, in-memory cache (e.g., Redis) that stores user's active connection details, such as the chat server they’re connected to and their last_active timestamp.

🔹 Notification Service - Sends push notifications via providers like FCM or APNS when users are offline.

🔹 Message Queue - Decouples real-time messaging from storage of the messages.

🔹 Message Storage Service - Consumes incoming messages from the Message Queue and persists them in the Message DB for efficient storage and retrieval.

🔹 Group Service - Responsible for handling all group-related functionalities, including creating groups, updating group details and returning list of group members.

🔹 Media Service - Handles the uploading and management of multimedia content, such as images, videos, and audio files.

🔹 Blob Storage - Storage backend for a chat application’s multimedia content (eg., S3).

🔹 CDN - To reduce latency when uploading or downloading multimedia content, files are distributed to locations geographically closer to users via a Content Delivery Network (CDN).

![image](https://github.com/user-attachments/assets/109b6b57-a0ee-4403-96bc-3744abfa0319)

You can read the detailed article on this system design interview problem here: https://blog.algomaster.io/p/design-a-chat-application-like-whatsapp

#### Learn Microservices
1. Microservices Architecture Basics: Monolithic vs. Microservices, characteristics (independence, scalability, resilience), and designing microservices boundaries (DDD-Domain-Driven Design)
2. Service Communication: Synchronous (REST, gRPC) vs. Asynchronous (Message Queues), API design and versioning, event-driven architecture, and event sourcing
3. Data Management: Database per service, distributed data management (saga pattern, 2PC, CQRS), and handling data consistency across services
4. Deployment Strategies: Containerization (Docker), orchestration (Kubernetes), and service discovery and registry (Eureka, Consul)
5. Frameworks and Tools: Spring Boot (Spring Cloud for microservices), Micronaut, Quarkus, or Dropwizard as alternatives
6. Communication Protocols: RESTful APIs and gRPC, messaging systems (Kafka, RabbitMQ)
7. Databases: SQL (PostgreSQL, MySQL), NoSQL (MongoDB, Cassandra), and distributed caching (Redis, Memcached)
8. CI/CD Pipelines: Tools like Jenkins, GitHub Actions, GitLab Cl, and deployment strategies like Blue-Green and Canary deployments
9. Infrastructure as Code: Terraform, Ansible, or AWS CloudFormation
10. Logging and Monitoring: Centralized logging (ELK Stack, Splunk) and monitoring tools (Prometheus, Grafana)
11. Resilience and Fault Tolerance: Circuit Breaker (Hystrix, Resilience4j), Bulkhead pattern, and retries
12. Security: OAuth2, OpenID Connect, and API Gateways (Zuul, Spring Cloud Gateway, Kong)
13. Testing Microservices: Unit and integration testing, contract testing (Pact), and end-to-end testing
14. Scalability Patterns: Horizontal and vertical scaling, load balancing (HAProxy, NGINX)
15. Distributed Tracing: Tools like Jaeger and Zipkin
16. Anti-Patterns: Avoiding distributed monoliths and over-engineering microservices

#### Bacnend Engineering
- System Design (scalability, microservices)
- APIs (REST, GraphQL, gRPC)
- Database Systems (SQL, NoSQL)
- Distributed Systems (consistency, replication)
- Caching (Redis, Memcached)
- Security (OAuth2, JWT, encryption)
- DevOps (CI/CD, Docker, Kubernetes)
- Performance Optimization (profiling, load balancing)
- Cloud Services (AWS, GCP, Azure)
- Monitoring (Prometheus, Grafana)

#### [Learn SQL Optimization – No More Slow Queries](https://x.com/Abhishekcur/status/1897709268662735091?t=YmPDxM6jk0CGchdYrx-CJw&s=08)
Slow SQL = Performance Bottlenecks = Lost Revenue. Optimize NOW

- Index Properly – Use B-Trees, Clustered, Covering, and Composite Indexes wisely
- Avoid `SELECT *` Fetch only necessary columns
- Use `EXPLAIN ANALYZE` – Identify slow operations & missing indexes
- Optimize Joins – Index Foreign Keys, use JOINs over subqueries
- Normalize for Integrity, Denormalize for Speed – Balance trade-offs
- Batch Inserts & Updates – Reduce write amplification
- Minimize Locks & Deadlocks – Use transactions efficiently
- Leverage Caching – Redis, Materialized Views, Query Cache
- Use the Right Data Types – Save space & improve indexing efficiency


### Resilience4j
**Resilience4j** is a lightweight fault tolerance library designed specifically for Java, enabling developers to build resilient applications. One of its key concepts is the **Bulkhead** pattern, which helps manage resources in a way that isolates failures and prevents a failure in one part of a system from cascading to others.

### What is the Bulkhead Pattern?

The **Bulkhead Pattern** is inspired by the design of ships that have multiple watertight compartments (bulkheads) to prevent water from flooding the entire ship if one compartment is compromised. In software design, this pattern involves partitioning resources in such a way that the failure of one component (e.g., service or thread pool) does not affect the overall system or other components.

### How Bulkheads Work in Resilience4j

1. **Resource Isolation**:
   - Bulkheads help to limit the number of concurrent requests to a particular service or resource. If that service or resource fails, it won’t deplete the resources (like threads) available for other services, allowing them to continue functioning.

2. **Implementation**:
   - In Resilience4j, bulkheads can be implemented using the **Bulkhead** decorator. This decorator creates separate thread pools, isolating the executions of different parts of a service. Each bulkhead has its own configuration for maximum concurrent calls and waiting limits.

3. **Configuration**:
   - You can configure bulkhead settings, such as:
     - **maxConcurrentCalls**: The maximum number of concurrent calls that are allowed to the service.
     - **maxWaitDuration**: The maximum time a call can wait if the limit of concurrent calls is reached before failing.

### Example of Using Bulkhead in Resilience4j

Here’s a basic illustration of how to use a bulkhead with Resilience4j:

```java
import io.github.resilience4j.bulkhead.Bulkhead;
import io.github.resilience4j.bulkhead.BulkheadConfig;
import io.github.resilience4j.bulkhead.BulkheadRegistry;

import java.util.function.Supplier;

public class ExampleService {
    
    private final Bulkhead bulkhead;

    public ExampleService() {
        // Create a BulkheadConfig with a maximum of 10 concurrent calls
        BulkheadConfig config = BulkheadConfig.custom()
            .maxConcurrentCalls(10)
            .maxWaitDuration(java.time.Duration.ofMillis(500))
            .build();

        // Create a BulkheadRegistry to manage Bulkhead instances
        BulkheadRegistry bulkheadRegistry = BulkheadRegistry.of(config);
        
        // Create a Bulkhead instance
        bulkhead = bulkheadRegistry.bulkhead("exampleBulkhead");
    }

    public String executeWithBulkhead() {
        // Decorate a supplier with the Bulkhead
        Supplier<String> decoratedSupplier = Bulkhead.decorateSupplier(bulkhead, this::doSomething);

        // Execute the decorated supplier
        return decoratedSupplier.get();
    }
    
    public String doSomething() {
        // Simulate some processing
        return "Processed Successfully!";
    }
}
```

### Advantages of Using Bulkhead in Resilience4j

1. **Isolation of Failures**: Prevents failures in one part of the system from affecting others, enhancing overall system resilience.
2. **Controlled Resource Management**: Helps manage system resources and provides predictable performance for critical services.
3. **Better User Experience**: Users can still access other parts of the application, even if one component is failing or under heavy load.

### Use Cases for Bulkhead Pattern

- **Microservices Architectures**: In microservices, where services could be using shared resources such as databases or third-party APIs, bulkheads can help isolate these calls.
- **High Traffic Applications**: In scenarios where certain services are expected to handle spikes in traffic, bulkheads help in controlling the load and ensuring that other services remain unaffected.

### Summary

In summary, the **Bulkhead pattern** in **Resilience4j** is a powerful way to enhance application resilience by isolating failures and controlling resource usage. By using bulkheads, you can ensure that the failure of one service does not bring down the entire application, maintaining better stability and reliability. This is particularly useful in distributed systems where multiple services interact and depend on one another.
