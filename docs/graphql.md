
### GraphQL
- GraphQL, a query language for APIs created by Facebook.
- GraphQL is a query language and execution engine tied to any backend service.

#### 1. GraphQL APIs have a strongly typed schema
A GraphQL schema is the backbone of every GraphQL API. It clearly defines the operations (queries, mutations and subscriptions) supported by the API, including input arguments and possible responses. 

GraphQL schemas are strongly-typed and can be written in the simple and expressive GraphQL Schema Definition Language (SDL). 
The developers don’t have to manually write API documentation any more — instead it can be auto-generated based on the schema that defines the API. 

#### 2. No more overfetching and underfetching
Developers often describe the major benefit of GraphQL with the fact that clients can retrieve exactly the data they need from the API. They don’t have to rely on REST endpoints that return predefined and fixed data structures. Instead, the client can dictate the shape of the response objects returned by the API.

This solves two problems commonly encounter with REST APIs: overfetching and underfetching.

> With GraphQL, the client can dictate the shape of the response objects returned by the API.

**Overfetching** means the client is retrieving data that is actually not needed at the moment when it’s being fetched. It thus drains performance (more data needs longer to be downloaded and parsed) of the app and also exhausts the user’s data plan.

A simple example for overfetching would be the following scenario: An app renders a profile screen for a user which displays the user’s name and birthday. The corresponding API endpoint that provides the information about specific users (.e.g /users/<id>) is designed in a way that it also returns the address and billing information about each user. Both are useless for the profile screen and therefore fetching them is unnecessary.

**Underfetching** is the opposite of overfetching and means that not enough data is included in an API response. This means the client needs to make additional API requests to satisfy its current data requirements.

#### 3. GraphQL enables rapid product development
GraphQL makes frontend developers’ lives easy. Thanks to GraphQL client libraries (like _Apollo_, _Relay_ or _Urql_) frontend developers are getting features like caching, realtime or optimistic UI updates basically for free — areas that could have entire teams dedicated to work on them if it wasn’t for GraphQL.

Increased productivity among frontend developers leads to a speedup in product development. With GraphQL, it is possible to completely redesign the UI of an app without needing to touch the backend.

#### Tools
- [GraphiQL: GraphiQL & the GraphQL LSP Reference Ecosystem for building browser & IDE tools.](https://github.com/graphql/graphiql)
- [GraphQL Faker](https://github.com/graphql-kit/graphql-faker)
