# 🤖 Smart Document Assistant (Advanced RAG)

An AI-powered system that allows users to upload PDFs and ask questions based on their content using **Retrieval-Augmented Generation (RAG)**.
The system combines **semantic search + LLM reasoning** to generate accurate, context-aware answers.

---

## 🚀 Features

### 📄 Document Processing

* Upload multiple PDF documents
* Extract text using PyMuPDF
* Intelligent text chunking with overlap

### 🔍 Advanced Retrieval (RAG)

* Semantic search using Sentence Transformers
* FAISS vector database for fast similarity search
* Keyword-based filtering for improved accuracy

### 🤖 LLM Integration

* Answer generation using Groq API (LLaMA model)
* Context-restricted prompting (reduces hallucination)

### 📊 Smart Enhancements

* ✅ **Confidence Score** (based on vector similarity)
* 📄 **Source Citation** (shows which PDF was used)
* 🔍 **Highlighted Answer** (important keywords in bold)
* 💬 **Chat Memory** (tracks previous interactions)

### 💾 Export Functionality

* Download generated answers as a `.txt` file
* Stores latest response dynamically

### 🖥️ User Interface

* Interactive UI built with Gradio
* Chat-style interface for better user experience

---

## 🧠 How It Works

1. User uploads PDF(s)
2. Text is extracted using PyMuPDF
3. Text is split into overlapping chunks
4. Chunks are converted into embeddings
5. Stored in FAISS vector index
6. User query is converted into embedding
7. Relevant chunks are retrieved
8. Chunks are cleaned and filtered
9. Context is sent to LLM (Groq)
10. Final answer is generated and displayed

---

## 🛠️ Tech Stack

* **Python**
* **Gradio** (UI)
* **FAISS** (Vector Search)
* **Sentence Transformers** (Embeddings)
* **Groq API (LLaMA)** (LLM)
* **PyMuPDF** (PDF Processing)
* **NumPy**

---

## 🧪 Testing

The system has been tested across:

* Functional scenarios (PDF upload, Q&A)
* Retrieval accuracy (semantic + keyword queries)
* Edge cases (empty input, no PDF, irrelevant queries)
* Feature validation (highlight, export, confidence score)

👉 See `testcases.md` for detailed test cases.

---

## ▶️ Run Locally

### 1. Install dependencies

```bash
pip install -r requirements.txt
```

### 2. Run application

```bash
python app.py
```

---

## 🔐 Environment Setup

Set your Groq API key:

```bash
export GROQ_API_KEY=your_api_key
```

---

## 📸 Screenshots

(Add screenshots here)

---

## 🌐 Deployment

This project can be deployed on:

* Hugging Face Spaces (Gradio)
* Streamlit Cloud
* Local environment

---

## 🚀 Future Improvements

* 📄 Highlight exact sentences from PDF
* 📊 Advanced confidence scoring
* 🔎 Hybrid search (BM25 + FAISS)
* 🧠 Conversational memory with context retention
* 📁 Multi-format support (PDF + DOCX + Images)

---

## 👨‍💻 Author

Keshav Goyal

---

## ⭐ Key Highlight

> This project demonstrates an end-to-end implementation of **Retrieval-Augmented Generation (RAG)** combining vector search and LLM reasoning for real-world document question answering.
