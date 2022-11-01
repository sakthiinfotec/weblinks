[Java Programming from uiowa.edu](http://user.engineering.uiowa.edu/~swd/LectureNotes/)  
[Java - Object-Oriented Programming: Polymorphism from uiowa.edu](http://user.engineering.uiowa.edu/~swd/LectureNotes/JavaHTP6e_10.pdf)  
[Java - Object-Oriented Programming from Java for Programming 2nd Edition - informit.com](https://www.informit.com/articles/article.aspx?p=1708679&seqNum=5)  
[developer.com - Diving Deeper into Polymorphism and its Benefits in Java](https://www.developer.com/design/diving-deeper-into-polymorphism-and-its-benefits-in-java/)  
[Abstract Factory Pattern - by androiddesignpatterns.com](https://www.androiddesignpatterns.com/2012/06/designing-for-backwards-compatibility.html)  

##### eBooks
[“Software Engineering at Google” curated by Titus Winters, Tom Manshreck and Hyrum Wright](https://abseil.io/resources/swe-book)  
[“Software Engineering at Google” curated by Titus Winters, Tom Manshreck and Hyrum Wright](https://abseil.io/resources/swe_at_google.2.pdf)  

##### Data Engineering
[Airbyte - Understanding Change Data Capture (CDC): Definition, Methods and Benefits](https://airbyte.com/blog/change-data-capture-definition-methods-and-benefits)  
[learnk8s.io - API gateway in Kubernetes & Service Mesh](https://learnk8s.io/kubernetes-ingress-api-gateway)  
[CQRS (command query responsibility segregation)](https://www.techtarget.com/searchapparchitecture/definition/CQRS-command-query-responsibility-segregation)  
[CQRS - Spring and Data Synchronization Between Queries and Commands](https://thenewstack.io/how-cqrs-works-with-spring-tools/)  

###### gRPC
```
* A High performance protocol built on top of HTTP/2
* Ideal for the communication between Microservices
* It's a modern, fast and efficient, built on top of HTTP/2, low latency, supports bi-directional Streaming, language independent, 
* Makes it super easy to plug in authentication, load balancing, logging and monitoring
* Clients open long lived connection to a gRPC server
* At the core, define messages and services using Protocol Buffers
* Supports timeout at client side, eventually cancels the request at server side
* Supports interceptor for Logging + Metrics in production environment
* It efficiently connects services in and across data centers with pluggable support for load balancing, tracing, health-checking, and authentication.
```

#### Microservices
[YouTube - What is gRPC? (Remote Procedure Calls)](https://www.youtube.com/watch?v=hVrwuMnCtok&ab_channel=StephaneMaarek)  
[YouTube - Protocol Buffers in gRPC](https://www.youtube.com/watch?v=yfZB2_rT_Pc)
[YouTube - gRPC & Protocol Buffer Introduction](https://www.youtube.com/watch?v=XRXTsQwyZSU&ab_channel=StephaneMaarek)  
[YouTube - Intro to gRPC: A Modern Toolkit for Microservice Communication (G)](https://www.youtube.com/watch?v=RoXT_Rkg8LA&ab_channel=Twilio)  
[YouTube - Introduction to gRPC: A general RPC framework that puts mobile and HTTP/2 first (M.Atamel, R.Tsang)](https://www.youtube.com/watch?v=hNFM2pDGwKI)  


#### General Technologies
* Relational databases

#### Web Technology
* Web Workers
* Web Sockets
* Web Components
* Shadow DOM
* Mobx
* Next.js
* FCP
* PWA
* Responsive Web Development
* Local Storage vs Session Storage vs Cookie
* Webpack (bundling/minification techniques)
* GraphQL
* Docker
* Accessibility and Security compliance
* Front-end performance optimisation
* TypeScript
* [API-first World](https://api-first-world.com/)  
* Chrome Developer Tools
* API Gateway
* AWS Lambda
* JWT
* OAuth 2.0, SAML, Open ID, SSO

#### Node.js
* Events
* Streams
* Express.js
* JavaScript testing frameworks (Jest, Enzyme, Mocha, etc.)

#### CSS
* SASS
* Media Queries
* Flexbox
* Grid Layout

#### JavaScript
* Method Binding
* Module (Default export & Named export)
* Iterator (Symbol Iterator)
* List iteration
* Generators
* Promise
* Automated Tests

#### React
* Components (Class & Functional)
* Pure Component
* Component Lifecycle phases (Initialization/Constructor, Mount, Update & Unmount) & methods
* HoC - Component transforms props into UI, But HoC transforms a component into another component
* Hooks (useState, useEffect, useCallback, useMemo, useLayout, useReducer, useRef) & 
* Custom Hooks - Reuse stateful logics between components / Alternative to HoC to some extent
* useEffect() - With / without deps
* useRef - Child nodes to trigger animations, select text, or manage the focus
* Rules for React Hooks
* Actions & Reducers
* JSX => Babel => React.createElement(name, props, value)
* Conditional Rendering
* Fragment
* Key in List Iteration
* Suspense & Eror Boundary
* State vs Props (Immutable, Passed from Parent to Child)
* Data passes Downwards + Event bubbles Upwards
* Lifting State up
* Context, Context Provider, Context Consumer, useContext() - For pass Props through nested components i.e props drilling
* Global State, Context, Redux Store
* Redux - Configure and use store
* Virtual DOM
* State Reconciliation (Diffing with DOM snapshot) using Fiber Engine
* SSR vs Server Side Component - Next.js
* Async operations using Saga vs Thunk
* RTK Query (Query, Mutation, transform, tags)
* React Router
* Lazy Loading Components
* Code Splitting - With code-splitting, React allows us to split a large bundle file into multiple chunks using dynamic import() followed by lazy loading these chucks when we need them with React.lazy
* React Testing Library and Cypress
