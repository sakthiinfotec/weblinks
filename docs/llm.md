#### [Explained: What powers ChatGPT and Bard? A look at LLMs or large language models](https://www.moneycontrol.com/news/business/explained-what-powers-chatgpt-and-bard-large-language-models-are-behind-the-incredible-human-like-interaction-10634791.html)

Large language models, or LLMs, are a type of AI model specifically designed to understand natural language.

Have you heard of ChatGPT? If you have not, it's an artificial intelligence (AI) chatbot that has taken the world by storm. It can write poems, code, and even novels. But what's powering generative AI models like OpenAI’s ChatGPT or Google’s Bard? It's all thanks to large language models (LLMs).

LLMs are a type of AI model specifically designed to understand natural language. It can process and generate text, allowing it to be used for a variety of tasks such as language translation, summarisation, and question-answering.

These models are trained on massive datasets that vary depending on the specific purpose of the LLM. Smaller datasets typically have tens of millions of parameters, whereas larger ones have hundreds of billions of data points.

In LLMs, parameters represent the ‘knowledge’ gained by the model during its training phase. More parameters generally result in more accurate predictions because the model has access to more contextual information. Some of the most prominent LLMs have hundreds of billions of parameters.

In simple terms, an LLM can be thought of as an enormous database of text data that can be referenced to generate human-like responses to prompts.

Let's do a little exercise to understand this better. Here's a sentence, and all you have to do is fill in the blank:

"I am going to the ____ to buy milk."

If your answer was "I am going to the store to buy milk", you are right. However, you could have also said "market" or "shop". There are quite a few possible answers to the sentence. If you were able to fill in the blank with something sensible, you just demonstrated how an LLM works.

##### What is LLM?
LLM is an AI system that specializes in understanding and generating human languages. It trained on the vast amount of text data allowing it to learn grammar, vocabulary, facts, and even some reasoning abilities. LLMs like GPT-3 use advanced algorithms to generate and predict the input they receive. They can be used in a wide range of applications such as answering questions, writing articles, summarizing text, and even creating poetry. As LLMs continue to evolve, they become increasingly powerful tools that can help us communicate effectively. LLM models are a breakthrough in Natural Language Processing (NLP), enabling machines to understand and generate human-like language. LLMs are built using Deep Learning techniques and trained on a vast amount of text data which allows them to recognize patterns and relationships within human language.

##### Use cases
They can then use this learning to perform a variety of tasks such as 
- Answering questions
- Generating text
- Language translation or even translation between languages

##### How does it work?

Language models rely on neural networks, which are machine-learning algorithms inspired by the human brain. These networks comprise interconnected nodes organized in layers, each processing information and transmitting it to the next layer.

For language models specifically, the neural network takes a word sequence as input and produces an output by predicting the most probable sequence of words.

##### How are LLMs trained?

The process of training an LLM can be divided into three stages: pre-training, fine-tuning, and inference.

During the pre-training stage, the model learns from vast amounts of text data including books, articles, and websites to understand how words work together and how sentences are built. It also figures out the meaning of words and learns the rules of grammar and how to put words in the right order. It does all of this by looking at patterns in the text, like how certain words often appear together.

After pre-training, the model can be trained for specific tasks like translating languages or answering questions. This is called fine-tuning, where the model learns more about the specific task it needs to do. It's like practicing a particular skill to get better at it.

Once the model is trained, the next stage is inference. The trained model can now be asked questions or given prompts, and it will generate answers or responses based on what it has learned during the pre-training and fine-tuning stages.

##### Which are the popular LLMs?

**GPT-3.5:** Generative Pre-trained Transformer-3.5 or GPT-3.5 is one of the largest LLMs developed by OpenAI and serves as the backbone for AI chatbot ChatGPT. Boasting an impressive 175 billion parameters, the model can carry out many tasks, such as text generation, translation, and summarisation.

**LaMDA:** Google's Language Model for Dialogue Applications (LaMDA) is the underlying technology behind the newly introduced Bard AI. This language model has undergone training using extensive conversational dialogue data, enabling it to grasp subtle linguistic nuances and engage in open-ended conversations. Google has also developed an advanced iteration called LaMDA 2, which is further refined and equipped to offer recommendations for user queries. LaMDA 2 incorporates Google's Pathways Language Model (PaLM), featuring an impressive parameter count of 540 billion.

**LLaMA:** Developed by Meta AI, the LLaMA model comes in various parameter sizes, ranging from 7 billion to 65 billion. Meta aims to democratize access to the field by introducing LLaMA, as the training of large models has traditionally been limited by the computational power required.

**WuDao 2.0:** Developed by the Beijing Academy of Artificial Intelligence, WuDao 2.0 is the largest model in existence, trained on 1.75 trillion parameters. WuDao 2.0 can simulate human speech and generate content.

**MT-NLG:** Megatron-Turing Natural Language Generation (MT-NLG), jointly developed by Nvidia and Microsoft, serves as the successor to Microsoft's Megatron-LM and Nvidia's Turing NLG 17B. These models underwent training on Nvidia's Selene ML supercomputer, utilizing a dataset consisting of 530 billion parameters. With its 105-layer deep neural network, MT-NLG can perform a wide range of natural language tasks, including completion prediction, reading comprehension, intelligent reasoning, language inferences, and more.

**Bloom:** BigScience Large Open-science Open-access Multilingual Language Model is an open-source LLM built by a consortium of over 1,000 AI researchers and trained on 176 billion parameters. The model is capable of generating text in 46 languages and code in 13 programming languages.

#### LlamaIndex
Llama Index is a data framework for building LLM applications, allowing users to use LLMs but on their private data. It consists of multiple tools to get, import, and ingest data into your application, like reading from APIs or PDfs or documents or SQL databases, and then it provides advanced retrieval and a query interface on that data. After that ingestion and building of these indices, it's usually followed by a step of generation where a generation model is presented with let's say, the question and retrieved answers and the model answers the question based on that retrieved data. 

#### Properties of LLMs
* Quantitative
  - Number of Parameters (i.e. ~ 10 - 100 Billian)
* Qualitative (
  - Emergent Properties (Zero-shot learning)
*Zero=shot Learning:* The capability of a machine learning model to complete a task it was not explicitly tainted to do.

### 3 Levels of using LLMs
*Level 1: Prompt Engineering*
*Level 2: Model Fine-tuning*
*Level 3: Build your own*

