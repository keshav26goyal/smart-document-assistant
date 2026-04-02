# 📄 Smart Document Assistant (Advanced RAG)

## 🚀 Overview
This project is a Retrieval-Augmented Generation (RAG) based system that allows users to upload PDFs and ask questions.

## ⚙️ Features
- Upload PDFs
- Semantic search using FAISS
- Context-based answering
- LLM integration (Groq API)
- Interactive UI using Gradio

## 🧠 How It Works
1. Extract text from PDF (PyMuPDF)
2. Split into chunks
3. Convert to embeddings
4. Store in FAISS
5. Retrieve relevant chunks
6. Send to LLM for answer generation

## 🛠️ Tech Stack
- Python
- FAISS
- SentenceTransformers
- Gradio
- Groq API

## ▶️ Run Locally
```bash
pip install -r requirements.txt
python app.py
