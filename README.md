![Final rag agent](https://github.com/user-attachments/assets/a88eae1f-4c51-4540-9d3d-29c377ed7d0a)![Pre data processing](https://github.com/user-attachments/assets/a066e2b0-2c07-4e0a-baac-07814a3f0f97)# 🧠 Python Notes RAG Chatbot using n8n, OpenAI & Pinecone

![Python](https://img.shields.io/badge/Python-Knowledge-blue)
![n8n](https://img.shields.io/badge/Automation-n8n-orange)
![OpenAI](https://img.shields.io/badge/AI-OpenAI-green)
![Pinecone](https://img.shields.io/badge/VectorDB-Pinecone-purple)

---

## 📌 Project Overview

This project is a **Retrieval-Augmented Generation (RAG) Chatbot** that answers questions using **Python notes as knowledge**.

The system automatically reads Python notes from Google Drive, processes them into searchable chunks, stores them in a **Pinecone vector database**, and allows users to ask questions through an **AI-powered chat agent**.

This project demonstrates:

- 🤖 AI-powered chatbot
- 📚 Knowledge-based search
- 🔍 Semantic search using embeddings
- 🗄️ Vector database storage
- ⚡ Workflow automation using n8n

---

## 🚀 Features

✅ Upload Python notes automatically  
✅ Split large documents into chunks  
✅ Convert text into embeddings  
✅ Store knowledge in Pinecone  
✅ Ask questions using chatbot  
✅ Retrieve relevant answers  
✅ Maintain conversation memory  

---

## 🏗️ Project Architecture

This project contains **two main workflows**.

---

### 📂 Workflow 1 — Knowledge Upload

Stores Python notes into Pinecone.
Google Drive Trigger
⬇
Download File
⬇
Default Data Loader
⬇
Recursive Character Text Splitter
⬇
OpenAI Embeddings
⬇
Pinecone Vector Store


---

### 💬 Workflow 2 — Chat Agent

Answers user questions using stored notes.

When Chat Message Received
⬇
AI Agent
⬇
OpenAI Chat Model
⬇
Simple Memory
⬇
Pinecone Vector Store


---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| **n8n** | Workflow Automation |
| **OpenAI** | Embeddings & Chat Model |
| **Pinecone** | Vector Database |
| **Google Drive** | File Storage |
| **Python Notes** | Knowledge Base |

---

## 📂 Project Structure
project/
│
├── workflows/
│ ├── knowledge-upload-workflow.json
│ ├── rag-chat-agent-workflow.json
│
├── data/
│ ├── python_notes.pdf
│
├── screenshots/
│ ├── workflow1.png
│ ├── workflow2.png
│
└── README.md

