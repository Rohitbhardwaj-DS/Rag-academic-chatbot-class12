📚 RAG Academic Chatbot (Class 12 Biology)
This project is a Retrieval-Augmented Generation (RAG) based chatbot that answers questions from academic PDF documents using LangChain, ChromaDB, and Groq LLM (LLaMA 3.1).
It allows users to query educational content (Class 12 Biology PDFs) and get context-aware, accurate answers.

🚀 Features
📄 Load PDF documents from a folder (docs_dir)
✂️ Split large text into manageable chunks
🔍 Convert text into embeddings using HuggingFace
🧠 Store embeddings in Chroma vector database
🤖 Retrieve relevant content and generate answers using LLM
📌 Provides contextual answers from documents

📂 Project Structure
Rag-academic-chatbot-class12/
│
├── docs_dir/
│   ├── 12. Ecosystem.pdf
│   └── 6. Evolution.pdf
│
├── vector_db/              # Stores embeddings
├── langchain.ipynb        # Main notebook
├── requirements.txt
└── README.md

⚙️ Installation

Install dependencies:

pip install -r requirements.txt

🔑 Setup API Key

Set your Groq API key:

import os
os.environ["GROQ_API_KEY"] = "your_api_key_here"

▶️ How It Works
Load PDFs using DirectoryLoader
Split documents into chunks
Generate embeddings using HuggingFace
Store embeddings in ChromaDB
Retrieve relevant chunks using similarity search
Generate answer using LLaMA 3.1 (Groq)

💡 Example Query
What does the document say about Adaptive radiation?
✅ Sample Output

Adaptive radiation is the evolution of different species from a common ancestor in a given geographical area. Examples include Darwin’s finches and Australian marsupials.
