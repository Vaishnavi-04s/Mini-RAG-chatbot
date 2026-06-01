# Mini RAG Chatbot

## Overview

This project implements a Retrieval-Augmented Generation (RAG) chatbot that answers questions based on the contents of a PDF document. The chatbot extracts text from a PDF, converts the text into embeddings, stores them in a FAISS vector database, retrieves relevant information using semantic search, and generates answers using Google's Gemini LLM.

## Features

* PDF text extraction
* Text chunking
* Embedding generation using Sentence Transformers
* FAISS vector database for similarity search
* Semantic retrieval of relevant document chunks
* Gemini-powered answer generation
* Interactive question-answering interface
* Retrieval-Augmented Generation (RAG) pipeline

## Tech Stack

* Python
* PyPDF
* Sentence Transformers
* FAISS
* Google Gemini API
* Jupyter Notebook / Streamlit

## Project Architecture

PDF Document
↓
Text Extraction
↓
Text Chunking
↓
Embedding Generation
↓
FAISS Vector Database
↓
User Question
↓
Semantic Search
↓
Relevant Context Retrieval
↓
Gemini LLM
↓
Final Answer

## Installation

### Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/RAGChatbot.git
cd RAGChatbot
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

## Required Libraries

```bash
pypdf
sentence-transformers
faiss-cpu
google-generativeai
numpy
streamlit
```

## Setup Gemini API Key

Create a Gemini API key from Google AI Studio and configure it in your project:

```python
import google.generativeai as genai

genai.configure(api_key="YOUR_GEMINI_API_KEY")
```

## How It Works

1. Upload or load a PDF document.
2. Extract text from all pages.
3. Split the text into manageable chunks.
4. Generate vector embeddings for each chunk.
5. Store embeddings in FAISS.
6. Convert the user query into an embedding.
7. Retrieve the most relevant chunks.
8. Send the retrieved context and question to Gemini.
9. Generate and display the final answer.

## Example Questions

* What is SQL?
* Explain normalization.
* What are joins in SQL?
* What is the purpose of indexing?

## Project Structure

```text
RAGChatbot/
│
├── app.ipynb
├── SQL_Lecture_Notes.pdf
├── requirements.txt
├── README.md
├── .gitignore
└── ragenv/
```

## Future Enhancements

* Support multiple PDF uploads
* Chat history memory
* ChromaDB integration
* Hybrid search (keyword + semantic)
* Streamlit web interface
* Source citation display

## Learning Outcomes

This project demonstrates:

* Retrieval-Augmented Generation (RAG)
* Vector databases
* Semantic search
* Prompt engineering
* Large Language Model integration
* Information retrieval techniques

## Author

Vaishnavi Sarva
