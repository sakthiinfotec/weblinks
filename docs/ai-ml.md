### AI -> ML -> ANN -> DL

#### [Activation Functions](https://www.v7labs.com/blog/neural-networks-activation-functions)
- Linear: Linear means something related to a line. All the linear equations are used to construct a line. Composition of linear functions will give linear result
- Non-Linear: A non-linear equation is such which does not form a straight line. 	A nonlinear equation forms an S-curve, bell curve or another nonlinear shape on a graph. Eg. Used to classify images

#### Popular Activation Functions
- [Rectified Linear Unit (ReLU)](https://www.kaggle.com/code/dansbecker/rectified-linear-units-relu-in-deep-learning/notebook): is an activation function that introduces the property of non-linearity to a deep learning model and solves the vanishing gradients issue. "It interprets the positive part of its argument. It is one of the most popular activation functions in deep learning. The function returns 0 if it receives any negative input, but for any positive value  x
  it returns that value back. So it can be written as f(x)=max(0,x).
- [Sigmoid](): This function takes any real value as input and outputs values in the range of 0 to 1.  The larger the input (more positive), the closer the output value will be to 1.0, whereas the smaller the input (more negative), the closer the output will be to 0.0
- Softmax
  
#### [Embeddings](https://blog.replit.com/chroma)
Just like traditional applications use databases to store and retrieve data, AI-powered applications need an AI native storage and memory layer. To work with models in the loop, data needs to be represented in an AI native way - using embeddings.

Embeddings are a numerical vector representation of all kinds of data, generated using an embedding model. When two pieces of data are similar in meaning, for example, two sentences that are about the same thing, their embeddings are close together in vector space.

By representing data in this way, we can interact with the data the same way we do with the models themselves. For instance, we can find the most relevant text documents for a specific question or topic, and then use them as the context for the LLM to answer the query accurately.

 - [Chroma](https://www.trychroma.com/) is the easiest to use embeddings store for an AI application. Chroma handles embedding documents and queries for you, and stores your documents alongside their embeddings. It supports filtering and dynamic updating out of the box, making it perfect for you next AI-powered application.

#### Vector Search
Vector Search feature, which opens up a whole new set of AI/ML driven use-cases:

🌟 Semantic Search  
🌟 Similarity Search  
🌟 Visual Search  
🌟 Recommendations  

**Vector Databases**

- Pinecone
- Weaviate
- Chroma
- Qdrant
- Typesense - used to build blazing-fast search experiences, faceted navigation experiences, geo-search, vector search, semantic search, similarity search and much more.

#### Glossary
 - Semantic search: Search based on meaning instead of specific words. It is the deep NLP encoding of sentences that gets the context and the meaning and so on.
