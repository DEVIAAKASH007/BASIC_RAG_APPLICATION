# 📚 Basic RAG Application

A Retrieval-Augmented Generation (RAG) application that allows users to ask questions about documents and receive relevant, context-aware answers using Large Language Models (LLMs).

## ✨ Features

- Upload and process PDF documents.
- Split documents into smaller chunks.
- Generate embeddings for document chunks.
- Store embeddings in ChromaDB.
- Retrieve relevant information using semantic search.
- Generate answers using an LLM based on retrieved context.

## 🏗️ RAG Workflow

```text
PDF Documents
      ↓
Document Loading
      ↓
Text Splitting
      ↓
Embedding Generation
      ↓
Vector Database (ChromaDB)
      ↓
User Query
      ↓

Relevant Context
      ↓
LLM
      ↓
Generated Answer
```

## 🛠️ Tech Stack

- **Language:** Python
- **Framework:** LangChain
- **Vector Database:** ChromaDB
- **Embeddings:** HuggingFace
- **LLM:** Google Gemini


## ⚙️ Installation

### 1. Clone the repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
cd YOUR_PROJECT_NAME
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Configure environment variables

Create a `.env` file:

```env
GOOGLE_API_KEY=your_api_key
```


## 📂 Project Structure

```text
Basic-RAG/
│
├── app.py
├── requirements.txt
├── .env
├── README.md
└── chroma_db/
```

## 🔄 How It Works

1. Upload a document.
2. Extract and split its text into chunks.
3. Convert chunks into vector embeddings.
4. Store embeddings in ChromaDB.
5. Convert the user query into an embedding.
6. Retrieve the most relevant chunks.
7. Pass the retrieved context to the LLM.
8. Generate a context-aware response.

## 🔐 Security

- Store API keys in environment variables.
- Never upload `.env` files or API credentials.
- Add sensitive files and generated databases to `.gitignore`.

## 👨‍💻 Author

**Kondapalli Aakash**

[GitHub](https://github.com/DEVIAAKASH007)

---

⭐ If you find this project useful, consider giving it a star!