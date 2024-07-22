# Gemma Model Document Q&A

This repository contains two Streamlit applications (`app1.py` and `app.py`) that use the Gemma model to answer questions based on the context provided in PDF documents. 

## Overview

- `app1.py`: Allows users to upload their PDF files, which are then processed to answer questions based on the content of the uploaded document.
- `app.py`: Uses preloaded PDF documents from a directory to answer questions based on their content.

## Features

- PDF document ingestion and vector embedding.
- Question answering based on document content using the Gemma model.
- Document similarity search to find relevant chunks of text.

## Requirements

- Python 3.8+
- Streamlit
- Langchain
- Langchain_groq
- Langchain_community
- Langchain_google_genai
- dotenv
- FAISS
- PyPDFLoader

## Setup

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/QA_RAG_GEMMA.git
   cd QA_RAG_GEMMA
