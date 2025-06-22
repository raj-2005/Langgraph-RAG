

<h1 align="center">🧠 RAG-Powered PDF Q&A Agent</h1>

<p align="center">
  <em>A LangGraph-based Retrieval-Augmented Generation (RAG) agent that answers questions from any PDF using LLMs, embeddings, vector search, and tools.</em>
</p>

---

## 🚀 What is This?

This project is a complete implementation of a **Retrieval-Augmented Generation (RAG)** agent using:

- 📎 A PDF document as the knowledge base  
- 🧠 A powerful **LLM (LLaMA3 70B)** via **Groq API**  
- 🔍 **ChromaDB** for local vector similarity search  
- 🧱 **LangGraph** for stateful, multi-step agent orchestration  
- 🔧 **LangChain Tools** to allow LLMs to retrieve relevant data

This is a **framework-agnostic, domain-agnostic** template to build scalable, document-aware LLM applications.

---

## 🧠 Why RAG?

RAG enhances LLMs by grounding their answers in **external factual data**. Instead of hallucinating, the model:

1. **Retrieves** relevant info (from a document/vector store)
2. **Reads and reasons** on top of it
3. **Responds** based on actual data

RAG ensures:
- Higher factual accuracy
- Lower hallucination
- Greater transparency
- Ability to cite sources

---

## 🧠 Architecture & Flow


---

## ⚙️ Core Components

| Component         | Role                                                         |
|------------------|--------------------------------------------------------------|
| `PyPDFLoader`     | Loads and parses the input PDF                              |
| `RecursiveCharacterTextSplitter` | Splits document into overlapping chunks     |
| `MiniLM Embeddings` | Transforms chunks into vector embeddings                  |
| `ChromaDB`        | Stores and indexes the document vectors                     |
| `LangChain Tool`  | Lets the LLM fetch info from the vector store               |
| `LangGraph`       | Controls the flow (LLM → Tool → LLM → Response)             |
| `Groq + LLaMA3`   | The core reasoning model                                    |

---



