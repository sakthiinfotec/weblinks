
### GraphQL
#### 1. GraphQL APIs have a strongly typed schema
A GraphQL schema is the backbone of every GraphQL API. It clearly defines the operations (queries, mutations and subscriptions) supported by the API, including input arguments and possible responses. 

GraphQL schemas are strongly-typed and can be written in the simple and expressive GraphQL Schema Definition Language (SDL). 
The developers don’t have to manually write API documentation any more — instead it can be auto-generated based on the schema that defines the API. 

#### 2. No more overfetching and underfetching
Developers often describe the major benefit of GraphQL with the fact that clients can retrieve exactly the data they need from the API. They don’t have to rely on REST endpoints that return predefined and fixed data structures. Instead, the client can dictate the shape of the response objects returned by the API.

This solves two problems commonly encounter with REST APIs: overfetching and underfetching.
