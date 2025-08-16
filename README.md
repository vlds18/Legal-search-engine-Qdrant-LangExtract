# Legal Facts Extraction and Semantic Search

This repository contains an end-to-end pipeline for extracting structured legal facts from case law documents, storing them in a vector database, and enabling intelligent semantic search with **LangExtract** and **LLM-powered summarization**.

The project combines **LangExtract, NLP, embeddings, Qdrant, and large language models (LLMs)** to provide a scalable legal knowledge base for research and applications such as:

- **Legal document search**  
- **Case law summarization**  
- **Property settlement and family law analysis**  
- **Domain-specific knowledge base auto-updating**  

---

## Features

- **Automated Fact Extraction with LangExtract**  
  LangExtract is used to parse raw case law text and automatically extract meaningful legal facts such as parties, case names, courts, orders, procedural history, and key legal concepts. This transforms unstructured legal documents into structured knowledge units that can be stored and queried efficiently.  

- **Vector Storage with Qdrant**  
  Each extracted fact is embedded into a high-dimensional vector and stored in Qdrant along with rich metadata (entity type, subject, evidence text, document reference). Qdrant’s powerful indexing enables fast semantic search at scale.  

- **Semantic Search**  
  Queries can be expressed in natural language and refined by entity type. For example, a user can search for “applications under Section 79 of the Family Law Act” and retrieve directly relevant facts, cases, and orders.  

- **Context Expansion**  
  When a fact is retrieved, surrounding context from the original case document is included to provide legal evidence in full sentences, making results more interpretable.  

- **Reranking**  
  A cross-encoder reranker improves search quality by scoring the semantic relevance of retrieved passages to the query, ensuring the most pertinent evidence appears first.  

- **LLM Summarization**  
  Retrieved results are passed to an LLM, which generates a **clean, professional legal summary** in plain English. The output reads like a legal brief—fact-focused, objective, and suitable for practitioners and students.  

---

## Why LangExtract + Qdrant is powerful

The real strength of this pipeline lies in the combination of **LangExtract and Qdrant**:  

- **LangExtract** ensures that unstructured legal judgments are broken down into precise, structured knowledge units. Instead of storing entire case documents, we store facts with clear entity labels.  
- **Qdrant** makes these facts searchable in a semantic space, so that queries like *“property settlement after divorce”* retrieve the most contextually relevant orders, parties, and case law—even if the exact wording doesn’t match.  

Together, they create a **scalable, intelligent legal search system** that goes beyond keyword-based retrieval, unlocking practical use cases in legal research, compliance, and decision support.  
