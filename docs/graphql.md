
### GraphQL
- GraphQL, a query language for APIs created by Facebook.
- GraphQL is a query language and execution engine tied to any backend service.
- The process of building a GraphQL API is vastly centered around the GraphQL schema. Hence, you’ll often hear the term schema-driven development in the context of GraphQL. It simply refers to a process where a feature is first defined in the schema, then implemented with resolver functions.

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

### Defining schemas: The Schema Definition Language
GraphQL has its own type language that’s used the write GraphQL schemas: The Schema Definition Language (SDL). In its simplest form, GraphQL SDL can be used to define types looking like this:

```graphql
type User {
  id: ID!
  name: String
}
```
The User type alone doesn’t expose any functionality to client applications, it simply defines the structure of a user model in your application. In order to add functionality to the API, you need to add fields to the root types of the GraphQL schema: Query, Mutation and Subscription. These types define the entry points for a GraphQL API.

For example, consider the following query:
```graphql
query {
  user(id: "abc") {
    id
    name
  }
}
```
This query is only valid if the corresponding GraphQL schema defines the Query root type with the following user field:
```graphql
type Query {
  user(id: ID!): User
}
```
So, the schema’s root types determine the shape of the queries and mutations that will be accepted by the server.

> The GraphQL schema provides a clear contract for client-server communication.

#### Concepts
**Schema stitching** is one of the newer ones in the GraphQL space. In short, schema stitching allows to combine and connect multiple GraphQL APIs and and merge them into a single one. Similar to how a React components can be composed out of existing ones, a GraphQL API can also be composed out of existing GraphQL APIs!

**GraphQL bindings** take the idea of schema stitching to the next level by enabling a simple approach to reusing and sharing GraphQL APIs.

#### GraphQL.js
Let’s take a quick tour through the functions that GraphQL.js provides. Note that its functionality is generally centered around a GraphQLSchema:

- `parse` and `buildASTSchema`: Given a GraphQL schema defined as a string in GraphQL SDL, these two functions will create a GraphQLSchema instance: const schema = buildASTSchema(parse(sdlString)).
- `validate`: Given a GraphQLSchema instance and a query, validate ensures the query adheres to the API defined by the schema.
- `execute`: Given a GraphQLSchema instance and a query, execute invokes the resolvers of the query’s fields and creates a response according to the GraphQL specification. Naturally, this only works if resolvers are part of a GraphQLSchema instance (otherwise it’s just restaurant with a menu but without a kitchen).
- `printSchema`: Takes a GraphQLSchema instance and returns its definition in the SDL (as a string).
Note that the most important function in GraphQL.js is graphql which takes a GraphQLSchema instance and a query — and then calls validate and execute:

```javascript
graphql(schema, query).then(result => console.log(result))
```

> To get a sense of all these functions, take a look at this simple node script that uses them in a straightforward example.

The graphql function is executing a GraphQL query against a schema which in itself already contains structure as well as behaviour. The main role of graphql thus is to orchestrate the invocations of the resolver functions and package the response data according to the shape of the provided query. In that regard, the functionality implemented by the graphql function is also referred to as a GraphQL engine.

#### Boilerplates
- [GraphQL Boilerplates: Collection of production-ready GraphQL boilerplate projects](https://github.com/graphql-boilerplates)

#### Tools
- [GraphiQL: GraphiQL & the GraphQL LSP Reference Ecosystem for building browser & IDE tools.](https://github.com/graphql/graphiql)
- [GraphQL Faker: It mocks the entire GraphQL API (based on its schema definition), so frontend and backend teams can work completely independently.](https://github.com/graphql-kit/graphql-faker)
- [Prisma](https://www.prisma.io/)
- [GraphQL Playground](https://github.com/graphcool/graphql-playground)
- [graphql-config](https://github.com/graphcool/graphql-config)
