# 📄 PDF RAG - Chat with Your Documents

A Retrieval-Augmented Generation (RAG) based application that allows users to upload PDF documents and ask questions about their content.

The application processes the uploaded PDF, retrieves the most relevant information from the document, and uses a Large Language Model (LLM) to generate accurate, context-aware answers.

---

## 🚀 Features

- 📤 Upload PDF documents
- 📖 Extract text from PDF files
- ✂️ Split documents into smaller chunks
- 🔍 Retrieve relevant document content based on the user's question
- 🤖 Generate answers using an LLM
- 💬 Ask multiple questions about the uploaded document
- 🔎 Context-aware question answering
- ⚡ Backend API for processing PDFs and generating responses

---

## 🧠 How RAG Works

This project uses the **Retrieval-Augmented Generation (RAG)** approach.

Instead of asking the LLM to answer questions only from its pre-trained knowledge, the system first retrieves relevant information from the uploaded PDF and provides that information as context to the LLM.

### RAG Pipeline

```text
PDF Upload
    ↓
Text Extraction
    ↓
Text Chunking
    ↓
Create Embeddings
    ↓
Store/Search Vectors
    ↓
User Question
    ↓
Similarity Search
    ↓
Retrieve Relevant Chunks
    ↓
LLM + Retrieved Context
    ↓
Generated Answer
