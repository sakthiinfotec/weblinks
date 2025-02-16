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

#### 3 Levels of using LLMs
*Level 1: Prompt Engineering*  
*Level 2: Model Fine-tuning*  
*Level 3: Build your own*  

#### LLM Models and Usecases
List of top models based on the task

- Code - Sonnet 3.5
- Images - Flux Pro
- Research on the Intenet - GPT-4
- RAG / in-context learning - GPT-4
- Video analysis - Gemini
- Video generation - Kling
- "Le Chat Robot": fine-tuned Mistral 7b to control robotic arms
- "Midistral": fine-tuned Mistral Small to create music
- "Alplex" : fine-tuned Mistral 7b for legal assistants
- 🔍Web Search: Search and get web links with @DuckDuckGo
- 🔥 Web Scraping: Get LLM-friendly markdown content from the URLs with @firecrawl_dev
- 🧩 Chunking: Organize data with @UnstructuredIO
- ✨ Embedding: Embed data with @MistralAI Embed.
- 🗂️ Vector database: Retrieve embeddings with @Qdrant_engine
- 🐫 Info Retrieval: Aggregate data using @CamelAIOrg's RAG.
- 🧠 Knowledge Graph: Generate with @CamelAIOrg's KG agents and store with @neo4j
- 🤖 Multi-Agent Role-Playing: Automate tasks with AI agents using @MistralAI Mistral Large 2
- 👀 Agent Monitoring: Use @AgentOpsAI to manage and oversee operations
- Music generation models: Suno and Limewire
- Ressearch: Grok and Perplexity AI
- [Fish Audio](https://x.com/FishAudio/status/1833787529595912531)
- [Fish Speech | TTS](https://speech.fish.audio/)
- [Pipio - The AI-powered video production platform](https://www.pipio.ai/)
- [SceneTex: High-Quality Texture Synthesis for Indoor Scenes via Diffusion Priors](https://daveredrum.github.io/SceneTex/)

Super intelligence is NOT going to be one model, it will an ensemble of models working together in concert

**Model Capabilities**  
- Analyze data
- Automate workflows
- Assistive experiences
- Explain concepts
- Programming assistance
- Summarize things
- Image generation
- Translate text in real time
- Interpret images and visuals
- Writing assistance
- Personalize content
- Predict trends

#### LLM Frameworks
An LLM application developer can face myriad of challenges such as using various foundation LLMs, consuming different data sources and vector stores, constraints on input/output data format, LLM token limits, unpredictability of LLM output, dynamic prompts, retaining the conversation context and so on.

LangChain is a simple and powerful framework for building applications that use large language models, such as ChatGPT, LaMDA or Claude2. LangChain offers abstraction to complex repetitive tasks so you can focus on building great applications, not on the plumbing.

#### Langchain
LangChain is a comprehensive Python library designed to streamline the development of LLM applications. By providing a structured framework and pre-built modules, LangChain empowers developers to efficiently organize and integrate various components of their LLM workflows, saving time and effort.

**Why Use LangChain?**
Here are the reasons why LangChain is helpful in building LLM applications:
- Combine multiple LLMs and services
- Automate complex workflows
- Integrate with data and systems
- Optimize cost and performance
- Ensure reliability and error handling
- Simplify deployment and monitoring

**What is LangChain?**
- LangChain is a framework for developing applications powered by large language models
- It makes the complicated parts of working and building with AI models easier
- As of August 2023, this game-changing library has already garnered almost 60,000 stars on GitHub

**Why LangChain?**
- Components: LangChain makes it easy to swap out abstractions and components necessary to work with language models 
- Customized chains: LangChain provides out-of-the-box support for using and customizing 'chains' - a series of actions strung together

**LangChain Components**
- Model I/O: Building blocks to interface with any language model
- Retrieval: Bridging external data with LLMs
- Chaining: Crafting complex LLM workflows with LangChain
- Memory: Retain context and refer to past interactions
- LangChain agents: Dynamic decision-making with LLMs
- Callbacks that run on events during execution

**Model I/O**
Building blocks to interface with any language model
The model is the core part of any large language model application. LangChain offers the necessary components to interface directly with any language model. Different components of model I/O:
- Prompts: Use a prompt template, select a prompt dynamically, and control model inputs
- Language models: Interface and make calls to LLMs through common interfaces
- Output parsers: Refine and extract valuable data from model outputs

**Retrieval: Bridging external data with LLMs**
Retrieval integrates real-time data with language models, reducing costly fine-tuning. It helps businesses ensure data relevance, cut costs, and produce timely responses.
Different components of retrieval:
- Document loaders: Load documents from many different sources
- Document transformers: Split documents, convert documents into Q&A format, drop redundant documents, and more
- Text embedding models: Take unstructured text and turn it into a list of floating-point numbers
- Vector stores: Store and search over embedded data.
- Retrievers: Query your data

**Memory**
Retain context and refer to past interactions
Memory is the concept of storing and retrieving data in a conversation. There are different types of memory. Memory is the concept of storing and retrieving data in a conversation. There are different types of memory:
- Buffer for storing all messages
- Buffer window for storing the last few interactions
- Entity memory for saving details about entities and learning more about them using an LLM.
- Using a knowledge graph to recreate the memory
- Summary for continuously condensed dialogue.
- Using vectorstore to store history and return relevant chat parts

**Chaining**
Crafting complex LLM workflows with LangChain
LangChain provides the 'Chain' interface, allowing users to link multiple LLMs or other components in sequence:
- Simplify complex applications: Convert intricate workflows into manageable steps
- Modularity: Easier debugging, maintenance, and scalability
- Create cohesive applications: Combine multiple operations for a unified user experience

**LangChain Agents**
Crafting complex LLM workflows with LangChain
- Agents autonomously accomplish goals by choosing actions
- More flexible than hardcoded action sequences
- Can handle complex tasks like assistants, game playing, automation
- The reasoning engine chooses the best actions dynamically
- A natural metaphor for goal-driven AI systems
- Can optimize sequences of actions toward a goal

**Callbacks**
Use callbacks for logging, monitoring, integrations, debugging, etc.
Benefits of using callbacks:
- Subscribe to events like start, new token, end, error
- Pass callbacks during initialization or requests
- Use for logging, monitoring, streaming, etc
- Built-in handlers available
- Integrations with 3rd party tools

#### RAG

![RAG Popeline](https://github.com/user-attachments/assets/106e2544-027a-4ef5-9781-1585543a4d27)

![AI Chatbot](https://github.com/user-attachments/assets/a7fc141e-af17-4c8c-8ce3-d3cc4a70836b)


The image outlines a process related to Large Language Models (LLMs) and Retrieval-Augmented Generation (RAG). Here’s a breakdown of the terminologies:

1. **Extract**: This step involves gathering data from various sources (e.g., documents, databases). The extracted data could come from different file formats like PDFs, Word documents, HTML, and more.
2. **Encode**: Once the data is extracted, it's transformed into a machine-readable format, typically represented as numerical vectors. This encoding allows the model to understand and process the information effectively.
3. **Index**: In this step, the encoded data is organized for efficient retrieval. Indexing involves creating a structured representation that facilitates quick access to relevant information during the retrieval phase.
4. **Retrieve**: When a query is made, the model retrieves relevant documents or pieces of information from the indexed data. This involves searching for and identifying data that matches the query context.
5. **Rerank**: After retrieving a set of candidate answers or documents, this step involves re-evaluating and ranking them based on relevance to ensure the most pertinent information is prioritized.
6. **Calibrate**: This step fine-tunes or adjusts the response based on additional factors, such as the context of the query or user preferences, to enhance the quality and relevance of the final answer.
7. **Answer**: The final output, which is generated based on the reranked information and calibration, providing the user with a concise and relevant response to their query.

This workflow showcases how LLMs and RAG techniques can be combined to handle complex queries by leveraging both generative and retrieval-based capabilities effectively.

- [Rockset: Hybrid Search Architecture](https://rockset.com/whitepapers/hybrid-search-architecture/)


##### Embedding Model
Google just released Gemma Embeddings!

"GemmaEmbed is a dense-vector embedding model, trained especially for retrieval. As of December 12, 2024, GemmaEmbed achieves the #1 position overall on the MTEB leaderboard, with a score of 72.72."
![image](https://github.com/user-attachments/assets/a5a8c547-f58d-42b0-afdf-3c370fcf329e)


#### AI Assistant
- Kind of agency - able to make decisions and work in autonomy
- A 24/7 customer service expert
- Your personal {domain} assistant /  finance assistant: Handles a wide array of queries, including refunds, returns, payment-related issues, cancellations, disputes, and invoice inaccuracies, ensuring swift and effective solutions.
- Multilingual chat support
- Voice assistants: AI voice assistants can be found in smartphones, smart speakers, and cars, and can perform a variety of functions, such as playing music, looking up facts, and controlling smart home devices.
- Image recognition for face unlock in mobile phones
- ML-based financial fraud detection
- Research assistant
- Text summarization and transformation
- Voice-to-Text and Text-to-Voice
- OCR
- Decision making (Credit / Risk management)

[Building websites / apps with AI](https://x.com/venturetwins/status/1889345133109285322)

![image](https://github.com/user-attachments/assets/aa1fa8b6-7985-4033-a809-8db6aa495b88)

#### [Google Gen AI Python SDK v1.0.0 is here!](https://x.com/patloeber/status/1888983994533867558)
It brings major improvements and stability, including:

- Gemini API and Vertex support
- pydantic types
- function calling
- JSON response schema
- streaming
- async
- Imagen 3 support
- finetuning

![image](https://github.com/user-attachments/assets/ff8cee8e-eda6-450f-8bb3-9d1b1186e99e)

Helpful resources:

- Repo: [https://github.com/googleapis/python-genai](https://github.com/googleapis/python-genai)
- Docs: [https://ai.google.dev/gemini-api/docs/quickstart?lang=python](https://ai.google.dev/gemini-api/docs/quickstart?lang=python)
- Migration guide from the old SDK: [https://ai.google.dev/gemini-api/docs/migrate](https://ai.google.dev/gemini-api/docs/migrate)

![image](https://github.com/user-attachments/assets/7bceff42-e45e-4e6e-9037-17b3d31317a7)


#### agent.ai by @dharmesh
- [FlyerScan](https://agent.ai/agent/flyer-scan)
  - [R-N Super markets](https://rnsupermarkets.com/)
  - [Shaws Weekly Ad](https://www.shaws.com/weeklyad)

#### AI Agent - Usercases
* Insurance: Help customers to file a claim or add someone to our Premium
* Consumer Electronics: Help in the Technical Support
* Telecom: Manage subscription, convince people not to cancel the subscription or upgrade or downgrade plans
* Supply Chain: Contact review by AI Agent
* Travel: Hotel, Flight booking
* Customer Service: Handle return or change of items
* OTT: Update the subscription

#### AI Agent - Benefits
- Bring down the cost of the personalized interaction
- Affords the opportunity to have an orders of magnitude more personalized conversations with customers
- Value propositions: Gevernance, Guardrails
- [Delight your customers while dramatically improving business outcomes](https://sierra.ai/product)

**Agents**  
An AI system that plans and performs tasks autonomously. Long running tasks, integrating repeatedly with environments, taking actions in the world.

_Key Characteristics:_
- Autonomous
- Goal-Driven
- Long Running
- Environmental Interaction

_Latest Features:_
- Multimodality
  * GPT-4o
    - Language
    - Image analysis
    - Image Generation
    - Vice transcription
    - Text-to-Speech
  * Sora
    - Video
- Reasoning  
- Deep Research
- Operators - Operating on a browser context on behalf of the user - Search content, Book Restaurant, Order food online
- Structured Outputs
  - Adhere to strict JSON schema
  - Reliable Type Safety
  - Very useful for the inter-agent communication
- Memory

_Types of Agents_
- Customer Service
- Financial Assistance
- Coding Agent - To solve complex coding problems (write, test and come back)
- Lots of agents will be around working on our behalf and talking to each other

[Ref: IIT Madras | Building the Intelligent Future - Shri. Srinivas Narayanan | Open AI](https://www.youtube.com/live/wRv7bLXkeXQ)

**Intuitive and authentic conversations**  
Your AI agent mirrors the nuances of human communication, ensuring seamless and organic customer service interactions while improving customer satisfaction.

- Deliver empathetic support: AI agents use language processing and human-level reasoning to create conversational interactions that are natural and satisfying
- Adapt to any inquiry: AI agents understand jargon, typos, and context to communicate with consideration, adapting to each customer's specific needs and emotions
- Respond in any language: AI agents communicate effortlessly in the language of users' choice for experiences that are personalized and inclusive
- No more menus: Move on from IVR systems and let your customers get straight to the resolution they need. With your AI agent, voice communication is fast and action is immediate—no more lengthy wait times or tedious touch-tone menus

**Beyond Q&A**  
Conversational AI isn’t just about answering questions. Your AI agent takes action to solve your customers’ problems, improving self-service resolution rate and average handle time
- Use your expertise: Your agent is informed by your knowledge base, and guided by your company’s policies and brand guidelines, enabling it to make informed decisions
- Take action, instantly: Your agent is connected to your systems of record - from your order management system to your CRM - so it can take action on your customer’s behalf, from processing an exchange, scheduling a delivery, updating a subscription, or changing a reservation
- Empower your teams: When your agent can’t solve your customer’s problem, it collects critical information and delivers a detailed summary to your customer service teams, preparing them to effectively manage escalations

**Anytime and anywhere**  
Your AI agent is up-to-date, delivering customer service anytime and anywhere to dramatically lower your response time.

- Around-the-clock: AI agents are available to handle customers' questions any time of day. Customers can put the conversation on hold if life takes them elsewhere, and your agent can pick up where they left off, later
- Connect across channels: Whether they're at home or on the go, offer your customers the convenience of support through both chat and voice
- Always-ready: AI agents are easy and low-cost to update, whether there is a new product to highlight, a new promotion to offer, or a new policy to follow
- Scalable: When you experience surges in consumer demand, Sierra scales up effortlessly, ensuring a smooth experience with plenty of capacity

**Always improving**  
Your agent is constantly learning from interactions, continuously improving, and keeping your team in-the-loop.

- Live summaries: Review actionable activity summaries across all conversations as they happen. Sophisticated pattern recognition allows you to spot small problems before they grow, whether identifying a common product question or flagging a shipping delay
- Automatic tagging: Agent tags and categorizes each conversation, making it easy to track success and see what your customers are interested in most.
- Integrated quality assurance: Monitor your AI agent's performance in real-time and make necessary adjustments. Sierra automatically flags conversations so your customer experience teams can focus on the interactions that need extra attention

#### Prompting
As shared by OpenAI President Greg Brockman.

Here’s how it works:
![image](https://github.com/user-attachments/assets/ce90b37c-8d8e-4bbe-a117-88348596eec9)

𝗧𝗵𝗲 𝗥𝗲𝗮𝘀𝗼𝗻𝗶𝗻𝗴

4 words in lowercase doesn’t work.

If you want to write a PRD, or a product strategy, or something for work, you have to help the LLM get your context. 

This is done in 4 parts.
𝗢𝗻𝗲 - 𝗚𝗼𝗮𝗹

LLMs know millions of ways to complete a task. 

Clear goal language helps them narrow in on the way you want them to. 

EG: “I want to create a Google-level Product Requirements Document for: <Feature>”

𝗧𝘄𝗼 - 𝗥𝗲𝘁𝘂𝗿𝗻 𝗙𝗼𝗿𝗺𝗮𝘁

The return format is really important, because there are so many styles.

Ideally, you can even create bespoke templates for bespoke tasks.

EG: “Our PRD template is: <Paste>” 

And the template has all the right headers and descriptions.

𝗧𝗵𝗿𝗲𝗲 - 𝗪𝗮𝗿𝗻𝗶𝗻𝗴𝘀

Tell the LLM what not to do as well as what to do. 

EG: “Prior PRDs that were too long or flowery were not well received. 

Focus on concise and specific to our app.”

Don’t assume it has your brain.
𝗙𝗼𝘂𝗿 - 𝗖𝗼𝗻𝘁𝗲𝘅𝘁 𝗗𝘂𝗺𝗽

This is where you paste in the user research, data, and meeting notes that you have. 

EG: “Here’s a transcript of a recent meeting where we finalized most of it”

You do have to be careful on not pasting too much.
