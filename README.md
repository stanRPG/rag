# RAG Local Project

A hands-on Retrieval-Augmented Generation (RAG) project for Udemy, demonstrating data ingestion, vector embeddings, and integration with OpenAI and HuggingFace models using LangChain and related libraries.

## Project Structure

```
RAG_local/
├── main.py                  # Entry point (prints hello message)
├── requirements.txt         # Python dependencies
├── pyproject.toml           # Project metadata and dependencies
├── .env                     # API keys (not tracked in git)
├── 0-DataIngestion/
│   ├── 1-DataIngestion.ipynb    # Notebook: data ingestion techniques
│   └── data/
│       └── text_files/
│           ├── machine_learning.txt
│           └── python_intro.txt
├── 1-VectorEmbeddings/
│   ├── embeddings.ipynb         # Notebook: intro to embeddings
│   └── openaiembeddings.ipynb   # Notebook: OpenAI embeddings usage
```

## Features
- Data ingestion from text, PDF, Word, Excel, and more
- Vector embeddings with OpenAI and HuggingFace
- Use of LangChain, FAISS, ChromaDB, and more
- Example notebooks for each step

## Setup
1. **Clone the repository**
2. **Install dependencies** (recommended: use a virtual environment):
	```bash
	pip install -r requirements.txt
	```
	Or with Poetry:
	```bash
	poetry install
	```
3. **Set up API keys**
	- Copy `.env.example` to `.env` and add your OpenAI API key:
	  ```env
	  OPENAI_API_KEY=your-openai-key-here
	  ```

## Usage
- Run the example notebooks in order:
  1. `0-DataIngestion/1-DataIngestion.ipynb` — Learn and try data ingestion
  2. `1-VectorEmbeddings/embeddings.ipynb` — Understand embeddings
  3. `1-VectorEmbeddings/openaiembeddings.ipynb` — Use OpenAI embeddings
- Or run the main script:
	```bash
	python main.py
	```

## Notebooks Overview
- **1-DataIngestion.ipynb**: Covers parsing and ingesting data from various formats for RAG systems.
- **embeddings.ipynb**: Explains what embeddings are and visualizes simple examples.
- **openaiembeddings.ipynb**: Shows how to use OpenAI's API for generating embeddings.

## Dependencies
Key packages:
- `langchain`, `langchain-openai`, `langchain-huggingface`, `faiss-cpu`, `chromadb`, `sentence-transformers`, `python-dotenv`, `pandas`, `matplotlib`, and more (see `requirements.txt` or `pyproject.toml`).

## Environment Variables
- `OPENAI_API_KEY` — required for OpenAI API access (set in `.env`)

## License
This project is for educational purposes (Udemy course).
