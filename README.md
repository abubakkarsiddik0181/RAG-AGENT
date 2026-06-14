# AI-Powered RAG Chatbot System with n8n, OpenAI & Pinecone

<img width="1020" height="576" alt="rag 1" src="https://github.com/user-attachments/assets/40cff07d-89fd-4d7d-8856-c412e390efaa" />
<img width="949" height="592" alt="rag 2" src="https://github.com/user-attachments/assets/18b2b30d-4147-4a68-a455-1d78c928cc21" />




An intelligent Retrieval-Augmented Generation (RAG) chatbot built with n8n. This system automatically ingests documents from Google Drive, generates embeddings using OpenAI, stores vectors in Pinecone, and enables users to chat with an AI agent that retrieves accurate answers from the knowledge base.

## Overview

This project consists of two workflows:

### Workflow 1: Knowledge Base Ingestion
Automatically monitors a Google Drive folder for new files and indexes them into Pinecone.

Process:
1. Detect new document in Google Drive
2. Download the file
3. Extract document content
4. Generate OpenAI embeddings
5. Store vectors in Pinecone

### Workflow 2: AI RAG Chatbot
Provides an AI-powered chatbot that retrieves relevant information from Pinecone and responds using OpenAI.

Process:
1. Receive user message
2. Search relevant knowledge from Pinecone
3. Maintain conversation memory
4. Generate contextual response using OpenAI
5. Return accurate answer to the user

---

## Features

- Automated document ingestion
- Google Drive integration
- OpenAI embeddings generation
- Pinecone vector database
- Retrieval-Augmented Generation (RAG)
- Conversational memory support
- AI Agent powered responses
- Scalable knowledge base architecture
- Low-code implementation using n8n

---

## Tech Stack

- n8n
- OpenAI GPT-4.1 Mini
- OpenAI Embeddings
- Pinecone Vector Database
- Google Drive API

---

## Architecture

```text
Google Drive
      │
      ▼
Document Upload
      │
      ▼
OpenAI Embeddings
      │
      ▼
Pinecone Vector Store
      │
      ▼
AI Agent
      │
      ▼
User Chat Interface
```

---

## Use Case

This system can be adapted for:

- Customer Support Chatbots
- Travel Agency Assistants
- Internal Knowledge Bases
- Company Documentation Search
- FAQ Assistants
- Product Information Bots

---

## Workflows Included

### Part 1 - RAG Knowledge Ingestion
- Google Drive Trigger
- File Downloader
- Document Loader
- OpenAI Embeddings
- Pinecone Vector Store

### Part 2 - AI Chatbot
- Chat Trigger
- OpenAI GPT Model
- Memory Management
- Pinecone Retrieval Tool
- AI Agent

---

## Results

- Automatically updates knowledge base when new documents are uploaded.
- Retrieves relevant information instead of relying solely on model memory.
- Provides more accurate and context-aware responses.

---

## Author

Built by Abu Bakkar Siddik.
Automation & AI Workflow Developer
