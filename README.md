# Fire Department RAG System

Source-linked RAG assistant for fire safety SOPs and medical response documents.

## Status: Week 2 of 3 - In Progress

### What's Working
- ✅ Document ingestion pipeline (PDF + Word)
- ✅ Chunking with semantic splitting
- ✅ Azure OpenAI embeddings (text-embedding-3-large)
- ✅ Vector storage in pgvector
- ✅ Basic semantic search

### Building Now
- 🔨 FastAPI backend
- 🔨 Citation extraction (page-level)
- 🔨 Query logging

### Next Week
- React frontend
- Response evaluation
- Deployment guide

## Architecture

PDFs/Word Docs → Ingestion Pipeline → Azure OpenAI Embeddings
↓
PostgreSQL + pgvector
↓
FastAPI Query API
↓
React Frontend

## Tech Stack
- **Embeddings:** Azure OpenAI (text-embedding-3-large)
- **LLM:** Azure OpenAI (GPT-4o-mini for dev, GPT-4o for prod)
- **Vector DB:** PostgreSQL 16 + pgvector
- **API:** FastAPI
- **Frontend:** React + Tailwind
- **Deployment:** Docker Compose

## Key Features
- Page-level citations with source documents
- Semantic search with metadata filtering
- Query logging for improvement
- Response thumbs up/down
- Refusal on low-confidence answers

## Hardware
- Development: RTX 3090 (24GB) for local testing
- Production: Azure OpenAI for inference
- Storage: Synology NAS for documents

## Cost
- Development: ~$20-30 in Azure OpenAI credits
- Target: <$0.10 per query in production

## Timeline
- Week 1: ✅ Ingestion + embeddings (DONE)
- Week 2: 🔨 API + citations (IN PROGRESS)
- Week 3: Frontend + docs (NEXT)

## Why This Project
Testing RAG patterns for operational knowledge where citation accuracy matters. 
Fire departments need fast, accurate answers with clear sources - wrong info can be dangerous.

---

## Setup (Coming Week 3)
Setup instructions will be added when the system is demo-ready.

## Contact
Arnaldo Sepulveda  
https://linkedin.com/in/arnaldo-sepulveda
