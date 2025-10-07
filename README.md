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

```bash
.
├── client.jac           # Web interface for chat and file uploads
├── server.jac           # Main application using Object Spatial Programming
├── server.impl.jac      # Implementation details and function bodies
├── mcp_server.jac       # Tool server for document and web search
├── mcp_client.jac       # Interface to communicate with tools
└── tools.jac            # Document processing and search logic
```

---

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
```

### 2️⃣ Install Dependencies

```bash
pip install jaclang jac-cloud jac-streamlit byllm langchain langchain-community langchain-openai langchain-chroma chromadb openai pypdf tiktoken requests mcp[cli] anyio
```

### 3️⃣ Set Up Environment Variables

```bash
export OPENAI_API_KEY=<your-openai-key>
export SERPER_API_KEY=<your-serper-key>
```

---

## 🏃 Running the Application

The application requires **three terminal windows** running simultaneously:

### Terminal 1: Start the MCP Tool Server

```bash
jac run mcp_server.jac
```

### Terminal 2: Start the Main Application

```bash
jac serve server.jac
```

### Terminal 3: Launch the Web Interface

```bash
jac streamlit client.jac
```

Once all three services are running, open your browser and navigate to:

```
http://localhost:8501
```

---

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
5. **Multimodal Understanding** — Images and videos are analyzed using **OpenAI's Vision models**.

---

## 🔧 Extending the Chatbot

The modular architecture makes it easy to extend:

- **New File Types** — Add support for audio, spreadsheets, or presentations
- **Additional Tools** — Integrate weather APIs, databases, or custom business logic
- **Enhanced AI Models** — Use different LLMs for specialized tasks
- **Advanced Search** — Implement hybrid search combining keyword and semantic search
- **Custom Chat Nodes** — Create specialized handlers for domain-specific questions

---

## 🛠️ Troubleshooting

### Dependencies Issues

Ensure all packages are installed and compatible with your Python version:

```bash
pip install --upgrade pip
```

### Server Startup Issues

Always start the MCP server (Terminal 1) before the main server (Terminal 2)

### File Upload Problems

- Check server logs for errors
- Verify file types are supported (PDF, TXT, PNG, JPG, MP4)
- Ensure files are not corrupted

### API Key Errors

Verify your environment variables are set correctly:

```bash
echo $OPENAI_API_KEY
echo $SERPER_API_KEY
```

### Port Conflicts

Ensure ports 8000, 8501, and the MCP server port are available

---

## 📚 Key Concepts

### Object Spatial Programming (OSP)

Organize your application as a network of interconnected nodes with walkers that traverse them, making complex logic intuitive and maintainable.

### Mean Typed Programming (MTP)

Let AI automatically classify and route data without writing complex rule-based logic. Simply define types and let the system handle classification.

### Model Context Protocol (MCP)

Build modular, reusable AI tools that can be shared across applications, promoting code reuse and maintainability.

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

---


## 🙏 Acknowledgments

Built with [Jac Language](https://www.jac-lang.org/) and powered by OpenAI's GPT models.

---

## 💬 Support

For issues and questions:

- Open an issue on GitHub
- Check the [Jac documentation](https://docs.jac-lang.org/)
- Visit the [Jaseci Labs repository](https://github.com/jaseci-labs)

