# RAG-BASICS

Retrieval-Augmented Generation (RAG) projects built with ChromaDB, SentenceTransformers, LlamaIndex and Gemini.

## Notebooks
- **Advanced_RAG_based_Article_Search.ipynb**: semantic search and Q&A over GeeksforGeeks articles
- **Basic_InterviewRag.ipynb**: RAG over interview questions (company and position based)

## Pipeline
1. Load and combine CSV data
2. Chunk text with LlamaIndex `SentenceSplitter`
3. Embed with `all-MiniLM-L6-v2` and store in a persistent ChromaDB collection
4. Retrieve the top-N similar chunks for a query
5. Build a grounded prompt and generate an answer with Gemini

## Setup
- Run in Google Colab with a GPU runtime
- Add your Gemini API key in Colab Secrets as `GOOGLE_API_KEY`
- Dataset: https://github.com/AshishJangra27/datasets
