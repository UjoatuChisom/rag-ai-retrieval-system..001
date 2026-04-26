# rag-ai-retrieval-system
LLM-powered Retrieval Augmented Generation (RAG) system using vector embeddings and Pinecone.

Problem

Large Language Models often hallucinate when answering questions because they lack access to structured and updated knowledge sources.

This project solves that problem by implementing a Retrieval Augmented Generation (RAG) system that retrieves relevant documents from a vector database before generating responses with an LLM.

The system allows organizations to query internal documents, knowledge bases, or datasets using natural language while maintaining accuracy and contextual relevance.

Architecture
User Query
   ↓
API Endpoint (FastAPI)
   ↓
Embedding Model (OpenAI Embeddings)
   ↓
Vector Database (Pinecone)
   ↓
Similarity Search
   ↓
Relevant Documents Retrieved
   ↓
LLM (OpenAI Chat Model)
   ↓
Context-Aware Response
Tech Stack

Backend

Python

FastAPI

AI

OpenAI API

Embeddings

Retrieval Augmented Generation (RAG)

Vector Database

Pinecone

Infrastructure

Docker

REST APIs

Automation

n8n (for workflow orchestration)

How to Run

Clone the repository

git clone https://github.com/UjoatuChisom/rag-ai-retrieval-system.git
cd rag-ai-retrieval-system

Install dependencies

pip install -r requirements.txt

Set environment variables

OPENAI_API_KEY=your_api_key
PINECONE_API_KEY=your_api_key

Run the API server

uvicorn main:app --reload

Access the API

http://localhost:8000
