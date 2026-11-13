# 📚 Custom Document RAG Question Answering System

<p align="center">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
  <img src="https://img.shields.io/badge/LangChain-1C3C3C?style=for-the-badge&logo=chainlink&logoColor=white" />
  <img src="https://img.shields.io/badge/ChromaDB-FF6F00?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Google%20Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white" />
</p>

<p align="center">
  <b>🤖 Ask questions. Retrieve knowledge. Get intelligent answers.</b>
</p>

A Python-based **Retrieval-Augmented Generation (RAG)** application that allows users to ask questions about their own PDF and TXT documents. Built using LangChain, ChromaDB, Hugging Face Sentence Transformers, and Google Gemini to deliver context-aware answers with source references and PDF page citations.

---

## ✨ Features

- 📄 **Document Loading** – Load custom PDF and TXT documents.
- ✂️ **Text Splitting** – Split documents using RecursiveCharacterTextSplitter.
- 🧠 **Local Embeddings** – Generate vector embeddings using Hugging Face Sentence Transformers.
- 🗄️ **Vector Database** – Store document embeddings in ChromaDB.
- 🔍 **Semantic Search** – Retrieve relevant document chunks using similarity search.
- 🤖 **AI-Powered Answers** – Generate contextual responses using Google Gemini.
- 📌 **Source Tracking** – Display source filenames and PDF page citations.
- ⚡ **Custom Knowledge Base** – Ask questions directly from your own documents.

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| 🐍 Python | Core programming language |
| 🔗 LangChain | RAG pipeline and document processing |
| 🗄️ ChromaDB | Vector database |
| 🤗 Hugging Face | Local text embeddings |
| ✨ Google Gemini API | AI-powered answer generation |
| 📑 PyPDF | PDF document extraction |

## 📂 Project Structure

```text
document_rag_project/
│
├── 📄 main.py
├── 📄 requirements.txt
├── 🔐 .env
│
├── 📁 documents/
│   ├── document1.pdf
│   └── document2.txt
│
└── 📁 chroma_db/
    └── Vector database storage
```

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/custom-document-rag-qa-system.git
```

### 2️⃣ Navigate to the Project Directory

```bash
cd custom-document-rag-qa-system
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Configure Environment Variables

Create a `.env` file in the root directory:

```env
GOOGLE_API_KEY=your_gemini_api_key
```

Get your API key from [Google AI Studio](https://aistudio.google.com/apikey).

### 5️⃣ Add Your Documents

Place your PDF and TXT files inside the `documents/` directory.

### 6️⃣ Run the Application

```bash
python main.py
```

## 🚀 How to Use

After running the application, select an option from the menu:

| Option | Action |
|---|---|
| `1` | 📥 Load documents and build the vector database |
| `2` | 💬 Ask questions about your documents |
| `3` | 🚪 Exit the application |

The system retrieves relevant document chunks and uses Google Gemini to generate answers based on the retrieved context.

## 🧠 How RAG Works

```text
📄 PDF / TXT Documents
        |
        ▼
  📥 Document Loading
        |
        ▼
  ✂️ Text Splitting
        |
        ▼
  🧠 Hugging Face Embeddings
        |
        ▼
  🗄️ ChromaDB Vector Storage
        |
        ▼
  🔍 Similarity Search
        |
        ▼
  📚 Retrieved Context
        |
        ▼
  ✨ Google Gemini
        |
        ▼
  💬 AI-Generated Answer
        |
        ▼
  📌 Source References
```

## 🔐 Security

- Keep your Google Gemini API key inside `.env`.
- Never commit `.env` to GitHub.
- Add `.env`, `.venv/`, and `chroma_db/` to `.gitignore`.

## 🎯 Project Goal

The goal of this project is to explore and implement Retrieval-Augmented Generation (RAG), combining local document processing, vector databases, semantic search, and Large Language Models to build a personalized document question-answering system.

## 👨‍💻 Author

**Savindu Hasintha**

- 💻 GitHub: [@savinduhasintha2005](https://github.com/savinduhasintha2005)

---

<p align="center">
  ⭐ If you find this project useful, consider giving it a star!
  <br/>
  <b>Built with ❤️ using Python and Generative AI</b>
</p>