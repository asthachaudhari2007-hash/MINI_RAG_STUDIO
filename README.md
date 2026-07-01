# 📚 Mini RAG Studio

An AI-powered **Retrieval-Augmented Generation (RAG)** application that allows users to upload PDF documents, build a vector database, and interact with the document using natural language. The project leverages **Google Gemini**, **LangChain**, **FAISS**, and **ChromaDB** to provide intelligent, context-aware responses.

---

## 🚀 Features

- 📄 Upload PDF documents
- ✂️ Automatic document chunking
- 🧠 Generate embeddings using Google Gemini
- 🗂️ Build vector databases using:
  - FAISS
  - ChromaDB
- 🔍 Semantic document retrieval
- 💬 Ask questions about uploaded documents
- ⚙️ Adjustable chunk size and chunk overlap
- 🎯 Configurable Top-K document retrieval
- 🖥️ Interactive Streamlit web interface

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Python | Programming Language |
| Streamlit | Web Interface |
| LangChain | RAG Pipeline |
| Google Gemini | Large Language Model |
| Google Generative AI Embeddings | Text Embeddings |
| FAISS | Vector Database |
| ChromaDB | Persistent Vector Store |
| PyPDF | PDF Processing |
| python-dotenv | Environment Variable Management |

---

## 📂 Project Structure

```text
Mini_RAG_Studio/
│
├── app.py
├── llm.py
├── .env
├── requirements.txt
│
├── data/
│   └── Uploaded PDFs
│
├── database/
│   ├── faiss_db/
│   └── chroma_db/
│
├── agents/
│   ├── note_agent.py
│   ├── quiz_agent.py
│   └── revision_agent.py
│
├── rag/
│   ├── loader.py
│   ├── splitter.py
│   ├── embeddings.py
│   ├── vectorstore.py
│   └── rag_chain.py
│
└── test/
    ├── test_loader.py
    ├── test_splitter.py
    ├── test_embedding.py
    ├── test_vectorstore.py
    └── test_rag.py
```

---

## ⚙️ Installation

### Clone the repository

```bash
git clone https://github.com/yourusername/Mini_RAG_Studio.git

cd Mini_RAG_Studio
```

### Create a virtual environment

```bash
python -m venv venv
```

Activate it

**Windows**

```bash
venv\Scripts\activate
```

**Mac/Linux**

```bash
source venv/bin/activate
```

---

### Install dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Configure Gemini API

Create a `.env` file in the project root.

```env
GOOGLE_API_KEY=YOUR_GEMINI_API_KEY
```

You can obtain your API key from:

https://aistudio.google.com/app/apikey

---

## ▶️ Run the Application

```bash
streamlit run app.py
```

The application will open in your browser at:

```
http://localhost:8501
```

---

## 🖥️ How to Use

1. Launch the application.
2. Upload a PDF document.
3. Select either **FAISS** or **ChromaDB**.
4. Adjust:
   - Chunk Size
   - Chunk Overlap
   - Top-K Results
5. Click **Build Database**.
6. Ask questions related to the uploaded document.
7. Receive AI-generated answers based on document content.

---

## 🔄 Workflow

```text
Upload PDF
      │
      ▼
Load Document
      │
      ▼
Split into Chunks
      │
      ▼
Generate Embeddings
      │
      ▼
Create Vector Database
      │
      ▼
Retrieve Relevant Chunks
      │
      ▼
Google Gemini
      │
      ▼
Generate Context-Aware Answer
```

---

## 📸 Application Preview

### Dashboard

- Upload PDF
- Configure chunking parameters
- Build Vector Database
- Ask questions
- Get AI-generated answers

*(Add screenshots here after uploading them to your repository.)*

---

## 🎯 Future Improvements

- Support multiple PDF uploads
- Chat history persistence
- Source citation highlighting
- Document summarization
- Export chat as PDF
- Voice-based document interaction
- Hybrid search (Keyword + Semantic)
- Multi-document comparison

---

## 📚 Learning Outcomes

This project demonstrates practical implementation of:

- Retrieval-Augmented Generation (RAG)
- Vector Databases
- Document Embedding
- Semantic Search
- Prompt Engineering
- Large Language Model Integration
- Streamlit Application Development
- LangChain Framework

---

## 🤝 Contributing

Contributions are welcome.

Feel free to fork the repository, create a feature branch, and submit a pull request.

---

## 📄 License

This project is developed for educational and learning purposes.

---

## 👩‍💻 Author

**Astha Chaudhari**

GitHub: https://github.com/asthachaudhari2007

---

⭐ If you found this project useful, consider giving it a star!