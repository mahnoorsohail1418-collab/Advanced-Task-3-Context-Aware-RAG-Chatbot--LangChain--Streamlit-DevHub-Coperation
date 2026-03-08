# Context-Aware Chatbot

## Objective

The objective of this project is to develop a **context-aware chatbot** that can answer user queries by retrieving information from a local knowledge base and maintaining conversation context.

Unlike simple rule-based chatbots, this system demonstrates how a chatbot can use **document retrieval and conversation history** to provide more relevant and coherent responses. The project is designed to illustrate fundamental concepts of **retrieval-based conversational AI** while keeping the implementation lightweight and easy to run in a **Jupyter Notebook environment**.

---

## Methodology / Approach

### 1. Knowledge Base Creation

A collection of `.txt` documents was created to serve as the chatbot's knowledge base.
These documents contain information on topics such as:

* Artificial Intelligence
* Machine Learning
* Deep Learning
* Natural Language Processing
* Python Programming
* Linear Regression

The chatbot loads these documents and processes them into smaller text chunks for easier retrieval.

### 2. Document Retrieval System

A simple retrieval mechanism was implemented to match user queries with relevant information in the knowledge base.

* Text is cleaned and tokenized
* Keywords from user queries are compared with document content
* The most relevant document segments are retrieved as responses

This simulates the basic concept behind **Retrieval-Augmented Generation (RAG)** systems.

### 3. Context Management

To support follow-up questions, the chatbot maintains a **conversation history**.

* Previous user queries are stored
* Context is used to interpret follow-up questions
* Responses become more relevant when users ask related questions

### 4. Chatbot Interface

Two interaction methods were implemented:

**Jupyter Notebook Interface**

* Built using `ipywidgets`
* Allows interactive conversation inside the notebook

**Streamlit Web Interface**

* A simple web-based chat interface
* Displays chat history and responses

### 5. System Components

The project consists of the following main modules:

* **Knowledge Base Loader** – loads and processes documents
* **Document Retriever** – finds relevant text segments
* **Chatbot Engine** – generates responses based on retrieved information
* **Conversation Memory** – stores chat history and context
* **User Interface** – notebook and web-based interaction

---

## Key Results / Observations

* The chatbot successfully retrieves relevant information from the knowledge base based on user queries.
* Context tracking allows the chatbot to handle **follow-up questions more effectively** than simple keyword-based systems.
* The lightweight implementation runs efficiently in **Jupyter Notebook without requiring large machine learning models**.
* Retrieval-based responses provide **accurate information when the relevant knowledge exists in the document database**.
* The Streamlit interface improves usability by providing a **clean web-based chat experience**.

### Insights

* Even simple retrieval systems can provide meaningful chatbot interactions when combined with context tracking.
* Expanding the knowledge base significantly improves response quality.
* This architecture can be extended with **vector embeddings, semantic search, and large language models** to build more advanced conversational AI systems.

Requirements

The project requires the following libraries:
Python 3.8+,
pandas,
numpy,
matplotlib,
seaborn,
torch,
torchvision,
scikit-learn,
joblib,
Pillow (PIL).


