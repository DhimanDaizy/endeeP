# AI Semantic Search & RAG System using Endee Vector Database

## Project Overview

This project demonstrates an **AI-powered semantic search system** built using the Endee vector database. The application allows users to upload PDF documents, automatically index them into vector embeddings, and ask natural language questions to retrieve relevant information from the documents.

The system implements a **Retrieval-Augmented Generation (RAG) pipeline**, where document chunks are embedded into vectors and stored in a vector database. When a user asks a question, the system retrieves the most semantically similar document chunks and returns the relevant information.

This project showcases practical AI infrastructure concepts such as vector databases, embeddings, semantic similarity search, and document-based question answering.

---

## Problem Statement

Traditional keyword-based search systems often fail to understand the **context and semantic meaning** of user queries. This makes it difficult to retrieve relevant information from large documents.

The goal of this project is to build a **semantic document search system** that can understand the meaning of a user's query and retrieve the most relevant information from uploaded documents.

---

## Key Features

* Upload PDF documents dynamically
* Automatic text extraction from PDFs
* Document chunking for better retrieval accuracy
* Embedding generation using transformer models
* Semantic similarity search
* Vector storage and retrieval using Endee
* Question answering interface
* Simple web-based UI using Flask

---
![alt text](image.png)

## System Architecture

User Interface (HTML + JavaScript)
↓
Flask Backend API
↓
PDF Upload & Text Extraction
↓
Document Chunking
↓
Embedding Generation
↓
Vector Storage in Endee
↓
Semantic Similarity Search
↓
Retrieve Relevant Context
↓
Return Answer to User

---

## Technologies Used

### Backend

* Python
* Flask

### AI / Machine Learning

* Sentence Transformers (for embeddings)

### Vector Database

* Endee Vector Database

### Document Processing

* PyPDF2

### Frontend

* HTML
* CSS
* JavaScript (Fetch API)

---

## How Endee is Used in This Project

Endee is used as the **vector database** to store and retrieve document embeddings.

Steps:

1. Extract text from uploaded PDFs.
2. Split text into smaller chunks.
3. Convert each chunk into vector embeddings.
4. Store embeddings in Endee.
5. Convert user queries into embeddings.
6. Perform similarity search in Endee.
7. Retrieve the most relevant document chunks.

This enables **semantic search instead of simple keyword matching**.

<img width="1313" height="646" alt="Screenshot 2026-03-13 191522" src="https://github.com/user-attachments/assets/f0022d8c-f99e-4e33-9fe6-aa1c9eae77bd" />


## Project Folder Structure

```
endeeP
│
├── app.py
├── semantic_search.py
├── pdf_indexer.py
├── embeddings.py
├── data_store.py
│
├── templates
│   └── index.html
│
├── uploads
│
└── README.md
```

---

## Installation & Setup

### Step 1: Clone the Forked Repository

```
git clone https://github.com/YOUR_USERNAME/endee.git
```

### Step 2: Navigate to the Project Folder

```
cd endee
```

### Step 3: Create Virtual Environment

```
python -m venv venv
```

Activate it:

Windows:

```
venv\Scripts\activate
```

Mac/Linux:

```
source venv/bin/activate
```

### Step 4: Install Dependencies

```
pip install flask PyPDF2 sentence-transformers numpy
```

---

## Running the Project

Start the Flask server:

```
python app.py
```

Open browser:

```
http://127.0.0.1:5000
```

---

## How to Use the System

1. Upload a PDF document.
2. The system extracts text and converts it into vector embeddings.
3. The embeddings are stored in the vector database.
4. Ask a question related to the uploaded document.
5. The system retrieves the most relevant document chunks using semantic similarity.
6. The result is displayed in the interface.

---

## Example Queries

* What is machine learning?
* Explain neural networks.
* What are the applications of artificial intelligence?

---

## Future Improvements

* Multi-document semantic search
* Chat-style conversational interface
* Highlighting answer sources
* Integration with large language models for better RAG responses
* Support for multiple file formats (PDF, DOCX, TXT)

---

## Conclusion

This project demonstrates a practical implementation of **semantic search and Retrieval-Augmented Generation using vector databases**. By leveraging embeddings and vector similarity search, the system can retrieve relevant information based on meaning rather than keywords.

The project highlights how modern AI systems use vector databases such as Endee to power intelligent search and document understanding applications.

---

## References

* Endee Vector Database Documentation
* Sentence Transformers Documentation
* Flask Documentation
* PyPDF2 Documentation

---
