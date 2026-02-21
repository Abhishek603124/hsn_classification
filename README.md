# HSN Trade Classification AI System  

An AI-powered **HSN Classification Assistant** built using **RAG (Retrieval-Augmented Generation)**, Knowledge Graphs, and Vector Search.

---

## Overview  

This project extracts structured HSN data from government trade PDFs, rebuilds hierarchical relationships (Chapter → Heading → Subheading → Item), and enables intelligent 8-digit HSN code search.

---

## System Pipeline  

### PDF Extraction  
- Extracted tabular data using `pdfplumber`  
- Cleaned and structured into Pandas DataFrame  

### Hierarchy Reconstruction  
- Restored Chapter → Heading → Subheading → Item  
- Enriched full contextual descriptions  

### Knowledge Graph  
- Built hierarchical graph using `NetworkX`  
- 2-digit → 4-digit → 6-digit → 8-digit mapping  

### Vector Search (FAISS)  
- Generated embeddings  
- Stored enriched descriptions  
- Enabled semantic similarity search  

### RAG Assistant  
- Built using LangChain + GPT-4  
- Handles exact match, code lookup, ambiguity clarification  

---

## Tech Stack  

Python • Pandas • pdfplumber • NetworkX • FAISS • LangChain • OpenAI GPT-4  

---

## Key Highlights  

- End-to-end data pipeline  
- Knowledge Graph design  
- Semantic search system  
- RAG-based controlled responses  
- Intelligent disambiguation logic  
