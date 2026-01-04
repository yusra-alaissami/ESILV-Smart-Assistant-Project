
# ESILV Smart Assistant

A multi-agent Retrieval-Augmented Generation (RAG) chatbot designed to provide accurate, source-grounded information about ESILV programs.  
The system uses local LLM inference, semantic search, and intelligent agent orchestration to ensure factual, privacy-preserving responses.

---

## Project Overview

The ESILV Smart Assistant combines:
- Local Large Language Models (LLMs) via Ollama
- Retrieval-Augmented Generation (RAG) using a vector database
- Multi-agent coordination with LangGraph
- A web-based chat interface built with Streamlit

The system supports cross-lingual retrieval (French documents, English queries) and handles both information requests and contact data collection through dedicated agents.

---

## Architecture Summary

- **User Interface:** Streamlit web application
- **Orchestration:** LangGraph for agent routing and state management
- **Agents:**
  - RAG Agent (information retrieval)
  - Form Agent (contact data collection)
- **LLM:** Local inference using `phi3:mini` via Ollama
- **Vector Store:** ChromaDB with multilingual embeddings
- **Data Source:** ESILV website content scraped with BeautifulSoup

---

## Setup Instructions

### Prerequisites
- Python 3.9+
- Google Colab or local environment
- Ollama installed
- Git

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yusra-alaissami/ESILV-Smart-Assistant-Project.git
cd ESILV-Smart-Assistant-Project

### How to use the ChatBOT 
- Ask questions about:
  - ESILV programs
  - Admissions and registration
  - Campus information

- The chatbot provides:
  - Context-aware answers based on retrieved documents
  - Source citations for transparency

