# 📄 Ask My PDF – Gemini-powered PDF Q&A App

Ask My PDF is a smart and intuitive Streamlit web application that lets you **upload PDF files and ask questions** based on their content. It uses **Google's Gemini 2.0 model** for high-quality answers and **FAISS** for fast semantic search. Ideal for students, researchers, and professionals who want to extract insights quickly from large documents.

---

## 🎥 Demo

![Demo of Ask My PDF](demo.gif)

> _The above GIF demonstrates the end-to-end functionality – from uploading the PDF to asking questions and getting instant answers._

---

## ✨ Features

- 📤 Upload one or multiple PDF files
- 💬 Ask questions in natural language
- ⚡ Fast, accurate, context-aware answers
- 📚 Splits and embeds large texts using LangChain
- 🔍 Efficient semantic search with FAISS
- 🤖 Powered by Gemini 2.0 Flash via `langchain-google-genai`

---

## 🚀 Getting Started

### 🔧 Prerequisites

- Python 3.8+
- A [Google API Key](https://makersuite.google.com/app/apikey)
- The following Python dependencies:
  - `streamlit`, `PyPDF2`, `langchain`, `faiss-cpu`, `python-dotenv`, `langchain-google-genai`, etc.

### 📦 Installation

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
pip install -r requirements.txt
```

Create a `.env` file in the root directory and add your API key:

```env
GOOGLE_API_KEY=your_gemini_api_key
```

---

### ▶️ Run the App

```bash
streamlit run app.py
```

---

## 🛠️ Tech Stack

| Layer         | Tech                           |
| ------------- | ------------------------------ |
| 🧠 LLM        | Gemini 2.0 (via Google GenAI)  |
| 💾 Vector DB  | FAISS                          |
| 📑 Embeddings | `embedding-001`                |
| 📚 Chunking   | RecursiveCharacterTextSplitter |
| 📄 PDF Parser | PyPDF2                         |
| 🌐 Frontend   | Streamlit                      |

---

## 📁 Project Structure

```
.
├── app.py              # Main Streamlit app
├── demo.gif            # GIF demo of the project
├── faiss_index/        # Local FAISS vector storage
├── .env                # Contains the Google API key
└── requirements.txt    # Python dependencies
```
