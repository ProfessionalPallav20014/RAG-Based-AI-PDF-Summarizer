# 📄 RAG-Based-AI-PDF-Summarizer

A fully local **Retrieval-Augmented Generation (RAG)** based AI system that performs PDF summarization and question answering using open-source HuggingFace models.

This project demonstrates the implementation of a complete RAG pipeline using **FAISS**, **Sentence Transformers**, and a locally loaded **Flan-T5** model — designed as a college-level experimental learning project.

---

## 🚀 Project Overview

This system allows users to:

- Upload a single PDF
- Generate a contextual summary
- Ask questions based on the PDF content
- Receive answers grounded in document embeddings

The entire pipeline runs locally using open-source models without relying on external APIs.

---

## 🧠 Tech Stack

| Component | Technology Used |
|------------|----------------|
| Embeddings | `sentence-transformers/all-MiniLM-L6-v2` |
| Vector Database | FAISS |
| Local LLM | `google/flan-t5-base` |
| Interface | Gradio |
| Framework | No backend framework (Notebook-based) |
| Execution Environment | Google Colab |

---

## 🏗️ Architecture

The project implements a custom class:


### RAG Pipeline Flow

1. **PDF Upload**
2. **Recursive Text Chunking**
3. **Embedding Generation**
4. **FAISS Index Creation**
5. **Semantic Retrieval**
6. **Answer Generation using Flan-T5**

All inference runs locally within the notebook session.

---

## ✨ Core Features

- 📂 Single PDF upload
- 🔍 Recursive text chunking
- 🧠 Local embedding generation
- 📚 FAISS-based semantic search
- 📝 Basic summarization
- ❓ Question answering over document
- 🖥️ Interactive Gradio interface
- 🔐 Fully local execution (no API keys required)

---

## 📦 Installation & Setup

This project runs entirely in **Google Colab**.

### Steps:

1. Open the provided notebook in Google Colab.
2. Run all cells sequentially.
3. All required dependencies are installed using `pip` within the notebook.
4. No `.env` file required.
5. No `requirements.txt` needed.
6. No specific Python version required (latest Colab runtime works).

---

## ▶️ How to Run

1. Open the notebook in **Google Colab**
2. Run every cell in order
3. Execute the final cell to launch the Gradio interface
4. A public link will be generated
5. Open the link in a new tab to interact with the application

---

## 📁 Project Structure

This project is intentionally minimal.


- All logic is implemented inside a single notebook.
- PDF upload is handled directly through the interface.

---

## 🎓 Intended Use

- College Project
- Experimental RAG Implementation
- Learning Resource for:
  - Vector Databases
  - Embedding Models
  - Local LLM Integration
  - Retrieval-Augmented Generation

---

## 🛠️ Models Used

- Embedding Model: `sentence-transformers/all-MiniLM-L6-v2`
- Language Model: `google/flan-t5-base`

Both models are loaded locally using HuggingFace transformers.

---

## 📌 Limitations

- Single PDF at a time
- Basic summarization (not abstractive multi-level)
- No persistent vector storage (session-based)
- Designed for demonstration and educational purposes

---

## 📈 Future Improvements (Optional Extensions)

- Multi-document support
- Persistent FAISS index
- Conversation memory
- Metadata filtering
- Deployment outside Colab
- Advanced prompt engineering

---

## 📷 Screenshots

_To be added_

---

## 📄 License

This project is developed for educational purposes.  
You may modify and extend it for personal or academic use.

---

## 🤝 Author

Developed as part of a college experimental AI learning project.
