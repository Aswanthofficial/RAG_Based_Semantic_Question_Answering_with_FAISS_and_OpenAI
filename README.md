# RAG_Based_Semantic_Question_Answering_with_FAISS_and_OpenAI

This project demonstrates a simple but powerful **Retrieval-Augmented Generation (RAG)** system using:
- 🔍 **FAISS** for semantic vector similarity search
- 🧠 **SentenceTransformers** for embedding sentences
- 🤖 **OpenAI GPT-3.5** to generate final answers based on retrieved context

The system retrieves top-k semantically similar sentences from a given corpus and feeds them into OpenAI's GPT model to generate a contextual and relevant answer.

---

## 📌 Key Components

| Component     | Technology                       |
|---------------|----------------------------------|
| Embedding     | `all-MiniLM-L6-v2` via `sentence-transformers` |
| Vector Search | FAISS                            |
| Language Model| OpenAI GPT-3.5 (`gpt-3.5-turbo`) |
| Input Type    | Simple sentence list (can be scaled to docs) |

---

## 🚀 Features

- Semantic similarity-based context retrieval
- Top-k FAISS search on dense embeddings
- OpenAI-powered context-aware response
- Easy to extend to documents, PDFs, or CSVs

---

## 🛠️ Installation

Install the required packages:

```bash
pip install faiss-cpu sentence-transformers openai
