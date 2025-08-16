Legal Facts Extraction and Semantic Search:

This repository contains an end-to-end pipeline for extracting structured legal facts from case law documents, storing them in a vector database, and enabling intelligent semantic search with LLM-powered summarization.

The project combines NLP, embeddings, Qdrant, and large language models (LLMs) to provide a scalable legal knowledge base for research and applications such as:

Legal document search

Case law summarization

Property settlement and family law analysis

Domain-specific knowledge base auto-updating

Features:

Automated Fact Extraction: Extracts entities, case names, courts, orders, and keywords from raw case law text.

Vector Storage with Qdrant: Embeds and stores extracted facts with metadata for fast retrieval.

Semantic Search: Search by natural language queries with optional entity filtering.

Context Expansion: Retrieves relevant surrounding text for each fact to provide richer evidence.

Reranking: Uses a cross-encoder reranker to improve retrieval quality.

LLM Summarization: Converts raw retrieved evidence into clean, professional legal answers.
