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
