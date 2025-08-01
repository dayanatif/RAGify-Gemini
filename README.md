# 🌟 RAGify-Gemini

A minimal yet powerful Retrieval-Augmented Generation (RAG) pipeline using **LangChain**, **Gemini 1.5 Pro**, and **Chroma** to fetch and answer queries based on live web data. Ideal for developers and researchers seeking a practical example of combining LLMs with vector-based retrieval.

---

## 📌 What is RAG?

**Retrieval-Augmented Generation (RAG)** is a technique that enhances the capabilities of language models by retrieving relevant external documents and using them to generate more accurate and grounded responses.

**RAG = Document Retriever + Language Model**

This approach is particularly useful when:
- The base LLM doesn't have access to real-time or domain-specific information.
- You need factual, up-to-date answers from dynamic sources.

---

## 🚀 Project Overview

`RAGify-Gemini` loads content from a real web page (Lilian Weng's Agent blog), splits it into chunks, stores it in a vector database using **Google Generative AI Embeddings**, and then uses **Gemini 1.5 Pro** to answer questions based on retrieved context.

---

## 📁 File Structure

ragify-gemini/
│
├── main.py # Full RAG pipeline using LangChain and Gemini
├── requirements.txt # All dependencies
├── README.md # You're here!


---

## 🔧 Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/dayanatif/ragify-gemini.git
   cd ragify-gemini

🛠️ Tech Stack
LangChain

Google Gemini 1.5 Pro

Chroma VectorDB

Google Generative AI Embeddings

BeautifulSoup4

Python 3.10+
