#### Python Cheatsheet
- [Python Cheatsheet - Github](https://github.com/gto76/python-cheatsheet)  
- [Python Cheatsheet - Zero To Mastery](https://zerotomastery.io/cheatsheets/python-cheat-sheet/)  

##### Python Stack
- [Pydantic - Data validation and settings management using Python type annotations](https://docs.pydantic.dev/)  
- [Celery - Distributed Task Queue](https://github.com/celery/celery)  
- [FastAPI - FastAPI framework, high performance, easy to learn, fast to code, ready for production](https://fastapi.tiangolo.com/)  
- [Starlette - A lightweight ASGI framework/toolkit, which is ideal for building async web services](https://www.starlette.io/)  
- [SQLModel - SQL databases in Python, designed for simplicity, compatibility, and robustness](https://sqlmodel.tiangolo.com/)
- [Beanie - Asynchronous Python object-document mapper (ODM) for MongoDB. Data models are based on Pydantic](https://beanie-odm.dev/)  
- [Typer - Build great CLIs. Easy to code. Based on Python type hints](https://typer.tiangolo.com/)  
- [Click - Python composable command line interface toolkit](https://github.com/pallets/click/)  
- [Jina AI - Jina is a MLOps framework](https://docs.jina.ai/)  
- [Jina AI - Build multimodal AI services via cloud native technologies·Neural Search·Generative AI·Cloud Native](https://github.com/jina-ai/jina)  
- [Cortex - ML Model serving at scale](https://github.com/cortexlabs/cortex)  
- [MkDocs - Write your documentation in Markdown and create a professional static site in minutes – searchable, customizable, for all devices](https://squidfunk.github.io/mkdocs-material/)  

##### Basics
- [Full Stack Python - Learn to Build, Deploy and Operate Python Applications](https://www.fullstackpython.com/)  
- [Python Crash Course for Non-Python Programmers - freecodecamp](https://www.freecodecamp.org/news/python-crash-course/)  
- [YouTube Chennels - Learn Python](https://towardsdatascience.com/top-13-youtube-channels-to-learn-python-524442aaab2f)  
- [Python for Machine Learning - Mini Course from *MachineLearningMastery*)](https://machinelearningmastery.com/python-for-machine-learning-7-day-mini-course/)  

#### API / Microservices**  
[Implement gRPC Server in Python](https://towardsdatascience.com/implementing-grpc-server-using-python-9dc42e8daea0)  

#### Flask | FastAPI  
- [Flask vs FastAPI](https://www.google.com/search?q=fastapi+vs+flask)  
- [Why we switched from Flask to FastAPI for production machine learning](https://towardsdatascience.com/why-we-switched-from-flask-to-fastapi-for-production-machine-learning-765aab9b3679)  
- [FastAPI alternatives](https://fastapi.tiangolo.com/alternatives/)  
- [Flask Tutorials (Deploy, Domain Name, SSL/TLS Certificate) - YouTube - Corey Schafer](https://www.youtube.com/playlist?list=PL-osiE80TeTs4UjLw5MM6OjgkjFeUxCYH)  

#### Data Engineering
- [Pathway: a Python ETL framework for stream processing, real-time analytics, LLM pipelines, and RAG | Powered by scalable Rust engine](https://github.com/pathwaycom/pathway)

#### Data Science
- [NumPy Tutorial – 2022](https://www.mygreatlearning.com/blog/python-numpy-tutorial)  
- JupyterLab or Binder
- [stlite: Serverless Streamlit | A port of Streamlit to WebAssembly, powered by Pyodide.](https://github.com/whitphx/stlite)
- [Pandas vs. FireDucks Performance Comparison: 20x faster Pandas by changing one line of code.](https://www.dailydoseofds.com/p/pandas-vs-fireducks-performance-comparison)

#### Computing
- [Dask - Dask is a flexible library for parallel computing in Python](https://docs.dask.org/en/latest/)  
- [Dask.distributed - A distributed task scheduler for Dask](https://distributed.dask.org/)  
- [Coiled - handles the creation and management of Dask clusters in the cloud](https://www.coiled.io/)  
- [Ray - Fast and Simple Distributed Computing](https://ray.io/)  
- [Apache Airflow - a platform to programmatically author, schedule and monitor workflows](https://airflow.apache.org/)  
- [Rapids.ai By NVDIA](https://rapids.ai/start.html)  
- [Vaex - a python library for lazy Out-of-Core DataFrames (similar to Pandas), to visualize and explore big tabular datasets](https://vaex.io/docs/index.html)  
- [Prefect — A modern, python-native data workflow engine](https://makeitnew.io/prefect-a-modern-python-native-data-workflow-engine-7ece02ceb396)  
- [Prefect IO - Dataflow Automation](https://www.prefect.io/)
- [FireDucks: Compiler Accelerated DataFrame Library for Python with fully-compatible pandas API](https://fireducks-dev.github.io/)

#### Best Practices
[Use a Flask Blueprint to Architect Your Applications](https://realpython.com/flask-blueprint/)  
[10 Must-Know Patterns for Writing Clean Code With Python - DZone](https://dzone.com/articles/10-must-know-patterns-for-writing-clean-code-with-1)  
- [Python naming convension for Class and Methods - StackOverflow](https://stackoverflow.com/questions/42127593/should-python-class-filenames-also-be-camelcased)  
- [PEP 8 – Style Guide for Python Code](https://peps.python.org/pep-0008/)  

#### Tools
* [uv - An extremely fast Python package installer and resolver, written in Rust](https://astral.sh/)
* [Ruff - An extremely fast Python linter and code formatter, written in Rust](https://docs.astral.sh/ruff)  
[sup - Stack Up](https://github.com/pressly/sup)  
[Go & Deep Learning tools by Ivan Zhang](https://github.com/1vn)  
[goose - DB migration tool](https://github.com/pressly/goose)  
[Cloud instance management for deep learning applications](https://github.com/for-ai/cloud)
[librosa - is a python package for music and audio analysis](https://librosa.org/doc/latest/install.html)  
[python-httpx - http2, requests + async http](https://www.python-httpx.org/)  
[Material for MkDocs - Write in Markdown and create a professional static site in minutes](https://squidfunk.github.io/mkdocs-material/) 
[Tenacity, a general-purpose retrying library, written in Python](https://tenacity.readthedocs.io/en/latest/)  

#### PythonAnywhere

[YouTube - Deploying Flask Apps Using Python Anywhere](https://www.youtube.com/watch?v=5jbdkOlf4cY&ab_channel=PrettyPrinted)  

```sh
cd flask_qa
pip freeze > requirements.txt
git init .
git add .
git commit -m 'initial commit'
```

In Console
```sh
git clone https://github.com/PrettyPrinted/flask_qa_app.git

# Create a virtual environment
mkvirtualenv env --python='/usr/bin/python3.8'

cd flask_qa_app
pip install -r requirements.txt
```

#### Popular packages
- pillow - The Python Image processing library
- openai
- python-dotenv
- retry
- fastapi - Includes Swagger UI
- uvicorn
- mangum
- pytest, mypy, pylint, isort, ruff, git, requests, factoryboy

