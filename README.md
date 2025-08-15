# MediBot – AI-Powered Medical Chatbot using RAG

MediBot is an AI-driven chatbot designed to answer medical queries by retrieving relevant information from domain-specific documents using Retrieval‑Augmented Generation (RAG). This project showcases the integration of vector databases, large language models (LLMs), and interactive UI components to solve real-world problems.

---

##  Features

- Retrieval‑Augmented Generation pipeline using LangChain  
- Context‑aware Q&A using Mistral‑7B or Groq‑hosted LLaMA model  
- FAISS‑powered vector search with HuggingFace embeddings  
- Real‑time chat interface built with Streamlit  
- Modular architecture for future enhancements  

---

##  Tech Stack

| Component      | Tool/Library                                |
|----------------|----------------------------------------------|
| Language Model | Mistral‑7B via HuggingFace / LLaMA via Groq  |
| Framework      | LangChain                                    |
| Embeddings     | HuggingFace (MiniLM‑L6‑v2)                   |
| Vector DB      | FAISS                                        |
| UI             | Streamlit                                    |
| Language       | Python                                       |
| Hosting        | AWS EC2 (optional)                           |

---

##  Project Structure

```bash
.
├── create_memory_for_llm.py       # Ingest PDFs and generate vector embeddings
├── connect_memory_with_llm.py     # Set up RetrievalQA with LLM and FAISS
├── medibot.py                     # Streamlit chatbot interface
├── data/                          # Input PDFs
├── vectorstore/                   # FAISS vector database
├── Pipfile / Pipfile.lock         # Pipenv environment files
├── requirements.txt               # Alternative install file
├── medical-chatbot-ppt.pdf        # Project summary presentation
└── README.md                      # This project documentation

## 🚀 Getting Started

### Install Dependencies

Using **Pipenv**:

```bash
pipenv install
pipenv shell



## 📥 Create the Vector Store

Add your PDFs to the `/data` folder, then run:

```bash
python create_memory_for_llm.py

