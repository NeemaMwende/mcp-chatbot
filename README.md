# 🤖 AI-Powered Multimodal MCP Chatbot

A sophisticated AI chatbot that can understand and interact with **documents**, **images**, and **videos** using **Jac's Object Spatial Programming (OSP)** and **Model Context Protocol (MCP)**.

---

## 🚀 Features

- **Multimodal AI Capabilities** — Chat with PDFs, text files, images, and videos
- **Intelligent Document Search** — Vector-based semantic search powered by **ChromaDB**
- **Web Search Integration** — Real-time information retrieval using **Serper API**
- **Vision AI** — Understand and discuss images and videos using **OpenAI's Vision models**
- **Smart Query Routing** — Automatic classification and routing using **Mean Typed Programming (MTP)**
- **Modular Architecture** — Clean separation of concerns with reusable **MCP tools**
- **User-Friendly Interface** — Built with **Streamlit** for easy interaction

---

## 🧰 Technologies Used

- **Jac Language** — Main application logic and Object Spatial Programming
- **Jac Cloud** — Backend server infrastructure
- **Streamlit** — Web interface
- **ChromaDB** — Vector database for document search
- **OpenAI GPT** — AI chat and vision capabilities
- **Serper API** — Real-time web search
- **LangChain** — Document processing and AI orchestration

---

## 🧱 Architecture Overview

The application uses **Jac's Object Spatial Programming (OSP)** paradigm with the following components:

- **Nodes** — Represent different parts of the system (Router, Chat types, Sessions)
- **Walkers** — Move through the node network, carrying information and executing logic
- **MTP (Mean Typed Programming)** — AI-based automatic classification and routing

---

## 🗂️ Project Structure

````bash
.
├── client.jac           # Web interface for chat and file uploads
├── server.jac           # Main application using Object Spatial Programming
├── server.impl.jac      # Implementation details and function bodies
├── mcp_server.jac       # Tool server for document and web search
├── mcp_client.jac       # Interface to communicate with tools
└── tools.jac            # Document processing and search logic

## ⚙️ Prerequisites

- **Python 3.12 or newer**
- **OpenAI API key**
- **Serper API key** (free tier available)

---

## 🧩 Installation

### 1️⃣ Clone the Repository
```bash
git clone <repository-url>
cd jac-mcp-chatbot

## 💡 Usage

### Step 1: Register or Log In
Create an account or log in through the web interface.

### Step 2: Upload Files
Upload **PDFs**, **text files**, **images**, or **videos** to the chatbot.

### Step 3: Start Chatting
Ask questions about your uploaded content or general queries.

### Step 4: Intelligent Routing
The system automatically routes your questions:

- 📄 **Document-related questions →** RAG (Retrieval-Augmented Generation) system
- 🌍 **General questions →** Web search
- 🖼️ **Image questions →** Vision AI
- 🎥 **Video questions →** Video content analysis

---

## 🔗 API Endpoints

| **Endpoint** | **Description** |
|--------------|-----------------|
| `POST /user/register` | Create a new user account |
| `POST /user/login` | Log in and get an access token |
| `POST /walker/upload_file` | Upload files (requires authentication) |
| `POST /walker/interact` | Chat with the AI (requires authentication) |

**Full API documentation available at:**
👉 [http://localhost:8000/docs](http://localhost:8000/docs)

---

## ⚙️ How It Works

1. **Document Processing** — Uploaded documents are processed and stored as vector embeddings in **ChromaDB**.
2. **Query Classification** — User queries are automatically classified using **Mean Typed Programming (MTP)**.
3. **Intelligent Routing** — Questions are routed to the appropriate handlers (RAG, web search, or vision AI).
4. **Context-Aware Responses** — The chatbot provides context-based answers from your data or real-time sources.
5. **Multimodal Understanding** — Images and videos are analyzed using **OpenAI’s Vision models**.
````
