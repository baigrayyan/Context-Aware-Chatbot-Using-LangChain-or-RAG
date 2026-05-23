# Context-Aware-Chatbot-Using-LangChain-or-RAG
This project implements a Retrieval-Augmented Generation (RAG) chatbot in Google Colab. It is designed to be context-aware, meaning it understands follow-up questions by considering the conversation history.

## 🚀 Features
- **RAG Architecture**: Uses external data (Wikipedia) to provide factual, up-to-date answers.
- **Contextual Retrieval**: Re-writes user queries to ensure standalone relevance using LangChain Expression Language (LCEL).
- **Hybrid Backend**: Uses local HuggingFace embeddings (`all-MiniLM-L6-v2`) to reduce API costs and Google Gemini Pro for high-quality chat completions.

## 🛠️ Tech Stack
- **Framework**: LangChain
- **LLM**: Google Gemini (via `langchain-google-genai`)
- **Embeddings**: HuggingFace (Local)
- **Vector Store**: FAISS
- **Data Loading**: WebBaseLoader (Wikipedia)

## 📋 Setup Instructions

1. **API Keys**: 
   - Get a free Google AI Studio API key.
   - In the Colab sidebar, click the **Secrets** (key icon).
   - Add `GOOGLE_API_KEY` and ensure the 'Notebook access' toggle is **ON**.

2. **Installation & Runtime**:
   - Run the installation cell.
   - **Restart the session** (Runtime -> Restart session) to load the new libraries.

3. **Execution**:
   - Run the 'Setup API Keys' cell to initialize environment variables.
   - Run the subsequent cells to load data, index documents, and start chatting.
