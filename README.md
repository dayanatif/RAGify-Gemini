
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

```plaintext
ragify-gemini/
│
├── main.py              # Full RAG pipeline using LangChain and Gemini
├── requirements.txt     # All dependencies
├── README.md            # You're here!
````

---

## 🔧 Setup Instructions

1. **Clone the repository**

   ```bash
   git clone https://github.com/dayanatif/ragify-gemini.git
   cd ragify-gemini
   ```

2. **Create and activate a virtual environment (optional but recommended)**

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set your environment variables**
   In `main.py`, set the following:

   ```python
   os.environ["LANGCHAIN_API_KEY"] = "your_langchain_api_key"
   os.environ["GOOGLE_API_KEY"] = "your_google_api_key"
   ```

5. **Run the app**

   ```bash
   python main.py
   ```

---

## 📥 Sample Output

```python
>>> rag_chain.invoke({'input':"What is MRKL"})
```

Output:

> MRKL stands for Modular Reasoning, Knowledge, and Learning. It is a framework used for building AI agents by combining different tools and decision-making mechanisms. MRKL enables more interpretable and modular AI systems.

---

## 🛠️ Tech Stack

* [LangChain](https://www.langchain.com/)
* [Google Gemini 1.5 Pro](https://deepmind.google/technologies/gemini/)
* [Chroma VectorDB](https://www.trychroma.com/)
* [Google Generative AI Embeddings](https://ai.google.dev/)
* [BeautifulSoup4](https://www.crummy.com/software/BeautifulSoup/)
* Python 3.10+

---

## 🌱 Future Improvements

* 🔄 Add file/document loaders (PDFs, CSVs, etc.)
* 🔍 Add more advanced retrieval methods (MMR, Hybrid Search)
* 💬 Streamlit UI for chat interface
* 🧠 Switch to long-context models (Gemini 1.5 Flash)
* 🧩 Add support for tool-using agents (e.g. MRKL agent)

---

## 📦 requirements.txt

```txt
langchain
langchain-google-genai
langchain-community
langchain-chroma
bs4
tqdm
```

---

## 🤖 Author

**Rao Dayan**
📍 AI & ML Enthusiast | LangChain Explorer
🔗 [LinkedIn](https://www.linkedin.com/in/dayanatif)
🛠️ Built with love, learning, and LangChain.

---

## 📌 Repository Info

* **Repo Name**: `RAGify-Gemini`
* **License**: MIT
* **Project Type**: Educational / Experimental
* **Status**: Actively maintained


## 🧠 Learn More

* [LangChain Documentation](https://docs.langchain.com/)
* [Gemini API Docs](https://ai.google.dev/)
* [What is RAG?](https://www.pinecone.io/learn/retrieval-augmented-generation/)

---


