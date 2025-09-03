# 🤖 AI powered contextual Document Chatbot  

An **AI-powered RAG (Retrieval-Augmented Generation) chatbot** that lets you interact with your own documents — PDFs, CSVs, Word files, or plain text — using advanced LLMs like **OpenAI GPT** and **Google Gemini**.  

This project merges **document retrieval** with **conversational AI**, enabling precise, context-driven responses while keeping your data private and local.  

---

## ✨ Key Highlights  

- 📂 **Flexible Document Support**  
  Upload and query multiple file formats: PDF, DOCX, CSV, and TXT.  

- 🔎 **RAG Workflow**  
  Combines embedding-based retrieval with generative models for reliable answers.  

- 🧾 **Conversation Memory**  
  Keeps track of past questions and answers to maintain context.  

- ⚡ **Local Vector Store**  
  Uses **ChromaDB** for fast and secure storage of embeddings.  

- 🔄 **Multiple LLM Backends**  
  Switch effortlessly between:  
  - **OpenAI GPT-3.5 / GPT-4**  
  - **Google Gemini Pro & Vision**  

- 🖥️ **Dual Interface**  
  - **Notebook** (`RAG_notebook.ipynb`) for experimentation  
  - **Streamlit app** (`RAG_app.py`) for production-ready UI  

- 🖼️ **Built-In Documentation**  
  Includes screenshots and architecture diagrams for easy reference.  

---

## 📂 Project Layout  

```text
Contextual-Doc-Chatbot/
├── RAG_app.py            # Streamlit-based chatbot UI
├── RAG_notebook.ipynb    # Step-by-step demo in Jupyter
├── requirements.txt      # Project dependencies
├── README.md             # Documentation
├── data/
│   ├── docs/             # Sample docs, images, diagrams
│   │   └── screenshots/  # UI captures
│   ├── tmp/              # Temporary uploads
│   └── vector_stores/    # ChromaDB local storage
```

---

⚙️ Getting Started
1. Clone the Repository
```bash
git clone https://github.com/yourusername/Contextual-Doc-Chatbot.git
cd Contextual-Doc-Chatbot
```

2. Install Requirements
```bash
pip install -r requirements.txt
```

3. Launch the App
```bash
streamlit run RAG_app.py
```

🏗️ System Overview

1. The chatbot is built on a Retrieval-Augmented Generation (RAG) pipeline, which works as follows:

2. Documents are split into chunks and embedded using OpenAI or Gemini embeddings.

3. Embeddings are stored locally in ChromaDB.

4. On query, the system retrieves the most relevant chunks.

5. An LLM (GPT or Gemini) generates an answer using both the retrieved context and conversation history.

---

🛠️ Tech Stack

--> LangChain – framework for RAG and conversational pipelines

--> ChromaDB – local vector database

--> OpenAI API – GPT models for text generation

--> Google Generative AI – Gemini for text + multimodal capabilities

--> Streamlit – simple, interactive frontend

--> Python 3.12

---

🧩 Core Modules
```bash
| File/Folder           | Purpose                                         |
| --------------------- | ----------------------------------------------- |
| `RAG_app.py`          | Streamlit interface for chatting with documents |
| `RAG_notebook.ipynb`  | Walkthrough of RAG pipeline                     |
| `data/vector_stores/` | Stores embeddings locally                       |
| `data/docs/`          | Contains test docs, diagrams, and screenshots   |
| `.env`                | Stores API keys securely                        |
```
---

🔒 Security & Privacy

✅ Local-first: Embeddings and vector stores are saved on your machine.

✅ Minimal exposure: Only relevant text chunks are passed to LLMs.

✅ Secure configuration: API keys are managed via environment variables.

---

📌 Summary

This project is a personal AI assistant for your documents, blending retrieval and generation seamlessly. With local storage, multiple LLM integrations, and a user-friendly interface, it’s both powerful and privacy-focused.
