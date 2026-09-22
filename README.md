# 🤖 Chatbot with RAG (Retrieval-Augmented Generation)

An intelligent chatbot built using **Streamlit, LangChain, and Groq LLM**, capable of answering user queries using both general knowledge and custom PDF data.

---

## 🚀 Features

* 💬 Interactive chatbot UI using Streamlit
* 🧠 LLM-powered responses (Groq - LLaMA3)
* 📄 PDF-based question answering (RAG)
* 🔍 Semantic search using embeddings
* ⚡ Fast and accurate responses

---

## 🏗️ Project Structure

* `phase_1.py` → Basic chatbot UI
* `phase_2.py` → LLM integration (Groq API)
* `phase_3.py` → RAG implementation with PDF

---

## 🧠 Tech Stack

* Python
* Streamlit
* LangChain
* Groq API (LLaMA3)
* HuggingFace Embeddings
* ChromaDB (Vector Store)

---

## ⚙️ Setup Instructions

### 1. Clone Repository

```bash
git clone https://github.com/vidhikarastogi/Chatbot-with-RAG.git
cd Chatbot-with-RAG
```

### 2. Install Dependencies

```bash
pip install streamlit langchain langchain-community langchain-groq huggingface_hub chromadb pypdf sentence-transformers
```

### 3. Set API Key

```bash
set GROQ_API_KEY=your_api_key   # Windows
```

### 4. Run Application

```bash
streamlit run phase_3.py
```

---

## 🔄 Project Pipeline

The working pipeline of the Chatbot with RAG system is as follows:

1. **User Input**

   * User enters a query through the Streamlit UI.

2. **Prompt Handling**

   * The input is processed and passed into the system prompt template.

3. **Embedding Generation**

   * The PDF document is split into smaller chunks.
   * Each chunk is converted into vector embeddings using HuggingFace models.

4. **Vector Store Creation**

   * Embeddings are stored in a vector database (ChromaDB).

5. **Similarity Search**

   * The system retrieves the most relevant chunks based on the user query.

6. **LLM Processing**

   * Retrieved context + user query is passed to the Groq LLM (LLaMA3).

7. **Response Generation**

   * The LLM generates an accurate, context-aware response.

8. **Display Output**

   * Response is displayed back in the Streamlit chat interface.

---

## 🔁 Workflow Diagram (Text Representation)

User Query → Streamlit UI → Embeddings → Vector DB → Retriever → LLM (Groq) → Response

---

## 📌 How It Works

1. Loads PDF document
2. Splits into chunks
3. Converts into embeddings
4. Stores in vector database
5. Retrieves relevant chunks
6. Generates answer using LLM

---

## 🎯 Use Cases

* Document-based Q&A
* AI assistants
* Knowledge base systems
* Study helper

---


## 👩‍💻 Author

**Nivedita Singh**
