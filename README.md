# Secure_Offline_RAG_System

### Developing a retrieval system using semantic vector search.

### Competition hosted on [Trustii.io](https://app.trustii.io/datasets/1529)

## Objectives of this challenge
Build a Flexible Local RAG System: Develop a RAG system that generates embeddings using an open-source LLM, the system must support local execution without relying on external API calls. The system should be flexible and capable of handling various types of text data, including but not limited to Q&A datasets, websites, code snippets, documentation, and more.

Create a Versatile Local Chat Interface: Build a chat interface that interacts with the vector store generated from text embeddings and stored locally. This interface should allow users to query embeddings and retrieve relevant information to generate responses through locally executed LLM. The interface should support interaction with different content types, multiple languages specifically handling queries in English and French, code snippets, etc demonstrating the system's flexibility.

## My Approach
- Created embeddings using the sentence-transformers model: multi-qa-MiniLM-L6-cos-v1.
- Built a FAISS HNSW index with the embeddings for efficient vector search.
- Retrieved the top 10 results using dense embeddings, created query-response pairs from these results, and re-ranked them using a cross-encoder model ms-marco-MiniLM-L-12-v2.
  
## How to Run
Simply follow the steps in the provided Jupyter Notebook.
