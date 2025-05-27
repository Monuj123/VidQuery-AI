# YT AnswerBot
A Retrieval-Augmented Generation (RAG) AI agent that answers questions using YouTube video transcripts.

# Overview
- This project is an AI-powered Q&A system that lets users ask questions about YouTube videos. It combines:
  - Real-time video scraping (Bright Data)
  - Vector search (PGVector + OpenAI embeddings)
  - LLM-powered responses (Anthropic Claude 3)
  - Stateful agent workflows (LangChain + LangGraph)

# Features
- YouTube Video Ingestion – Automatically fetches and stores transcripts.
- Conversational AI – Claude 3 generates natural, context-aware answers.
- React Frontend – Clean, interactive chat interface.

# Tech Stack
- Backend	- Node.js, Express.js, PostgreSQL (PGVector)
- AI/ML	- LangChain(tools, retrieval), LangGraph (agent), Claude 3, OpenAI embeddings
- Data Pipeline	- Bright Data (YouTube scraping)
- Frontend	- React (TypeScript), CSS

# Setup
- Prerequisites
  - Node.js (v18+)
  - PostgreSQL (with PGVector extension)
- API keys:
  - OpenAI (for embeddings)
  - Anthropic (Claude 3)
  - Bright Data (YouTube scraping)

# Installation
- Clone the repo
  
       git clone https://github.com/yourusername/VidQuery_AI.git
       cd VidQuery_AI
  
- Set up environment variables

         DB_URL=postgresql://user:pass@localhost:5432/VidQuery_AI
         OPENAI_API_KEY=your_key
         ANTHROPIC_API_KEY=your_key
         BRIGHTDATA_API_KEY=your_key
      
- Run the backend
  
         cd server
         npm install
         npm start  # Starts Express server at http://localhost:3000
  
- Run the frontend
  
         cd client
         npm install
         npm run dev  # Starts React app at http://localhost:5173
