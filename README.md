# RAG Document Chatbot using Flowise

This project implements a **Retrieval Augmented Generation (RAG) based AI chatbot** that can answer questions from uploaded documents.

The system processes documents, converts them into embeddings, stores them in a vector database, and retrieves relevant information to generate accurate responses.

Built using **Flowise AI**, **Mistral AI**, and **Google Gemini Embeddings**.

---

##  Features

- Document Question Answering
- Retrieval Augmented Generation (RAG)
- Conversational AI with memory
- Vector Search for accurate document retrieval
- Context-aware responses
- Easy visual pipeline using Flowise

---

##  Technologies Used

- Flowise AI
- Mistral AI (LLM)
- Google Gemini Embeddings
- Vector Store (In-Memory)
- Retrieval QA Chain
- Node-based AI workflow

---

##  Project Workflow

The chatbot pipeline works as follows:

1. **Document Loading**
   - Files are loaded using the File Loader node.

2. **Text Splitting**
   - Large documents are split into smaller chunks using Recursive Character Text Splitter.

3. **Embedding Generation**
   - Google Gemini Embeddings convert text into vector representations.

4. **Vector Storage**
   - Embeddings are stored in an In-Memory Vector Store.

5. **Retrieval**
   - Relevant chunks are retrieved based on the user query.

6. **Response Generation**
   - Mistral AI processes the retrieved context and generates an answer.

7. **Conversation Memory**
   - Buffer Memory stores chat history for contextual conversations.

---

##  Architecture

User Question  
↓  
Retriever (Vector Store)  
↓  
Relevant Document Chunks  
↓  
Mistral AI Model  
↓  
Generated Answer

---

##  Flowise Nodes Used

- Recursive Character Text Splitter
- File Loader
- Google Gemini Embeddings
- In-Memory Vector Store
- Mistral AI Chat Model
- Conversational Retrieval QA Chain
- Buffer Memory

---

##  Files Included

- `RAG CHATBOT Chatflow.json` → Flowise chatbot workflow

---

## How to Use

1. Install **Flowise AI**
2. Import the provided **Chatflow JSON**
3. Configure API Keys
   - Google Gemini API
   - Mistral AI API
4. Upload your document
5. Start asking questions

---

## Use Cases

- Document Q&A systems
- Research assistants
- Company knowledge base chatbot
- Student study assistant
- PDF based chatbot

---<img width="1907" height="864" alt="Screenshot 2026-04-08 094704" src="https://github.com/user-attachments/assets/c9140a60-83bb-448e-8320-4b771c1d3d95" />


## Future Improvements

- Persistent Vector Database (Pinecone / Chroma)
- Web interface
- Multi-document support
- Better memory management

---

## Author

Tamanna

---

If you like this project, consider giving it a star!
