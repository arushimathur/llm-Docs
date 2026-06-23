Steps - 

  # Install Ollama from ollama.com, then:
  1. ollama pull llama3.2
  2. ollama serve
  3. ollama run llama3.2
  
  Next install below - 

  pip install langchain langchain-community chromadb sentence-transformers ollama

  In simple terms, this command:

```bash
pip install langchain langchain-community chromadb sentence-transformers ollama
```

downloads and installs Python tools for building an AI chatbot that can use a local LLM like Llama.

* **langchain** → Helps connect all the AI components together.
* **langchain-community** → Extra integrations and connectors for LangChain.
* **chromadb** → Stores knowledge/documents so the AI can search them later.
* **sentence-transformers** → Converts text into numerical vectors (embeddings) that AI can search efficiently.
* **ollama** → Lets your Python code talk to locally running models such as `llama3.2`.

A simple way to think about it:

```text
Your Documents
      ↓
sentence-transformers (creates embeddings)
      ↓
chromadb (stores and searches them)
      ↓
langchain (orchestrates everything)
      ↓
ollama + llama3.2 (generates answers)
```

So this single command installs the building blocks needed to create a local AI assistant that can answer questions from your own documents.
