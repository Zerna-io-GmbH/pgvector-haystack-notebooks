# Integrating Pgvector and Haystack for Educational Purposes

Welcome to our educational repository, where we explore the integration of `pgvector` and `haystack` through Jupyter Notebooks for various easy-to-follow scenarios. This project is designed to provide step-by-step instructions and examples for embedding and retrieving data with PostgreSQL and leveraging local LLM technologies for educational purposes.

## Structure

- `files`: This folder contains example input files that are used in the notebooks for embedding into a PostgreSQL database with the `pgvector` extension.
- `notebooks`: This folder contains Jupyter Notebooks that serve as examples for how to integrate `pgvector` with Local LLM models and `haystack`.

## Example Notebooks

- **01_pgvector_connection**: Demonstrates the process of using `haystack` to embed data and store it in a PostgreSQL database using `pgvector`.
- **02_pgvector_retriever**: Demonstrates the process of using `haystack` and `PgvectorEmbeddingRetriever` to run queries on a PostgreSQL database.
- **03_pgvector_retriever_pipeline**: Demonstrates the process of using `haystack` and `PgvectorEmbeddingRetriever` to run queries on a PostgreSQL database and connect everything in a pipeline.
- **04_pgvector_ollama_embedder**: Demonstrates the process of using `haystack` and `ollama` embedding api to generate vector representations.
- **05_pgvector_ollama_embedder_pipeline**: Demonstrates the process of using `haystack` and `ollama` embedding api to generate vector representations and connect everything in a pipeline with various document cleanups and pdf file load.
- **06_pgvector_ollama_complete_process_pdf_embedding_query_generator**: Demonstrates the process of using `haystack`, `ollama`, `pypdf` to clean a pdf file. Embedd the context into a PostgreSQL database. Then it uses a `ollama` pipeline to run a query against `pgvector` and generate a LLM response.

## Docker Compose Setup

To simplify the setup process, we provide a Docker Compose file that runs a containerized PostgreSQL database with the `pgvector` extension pre-installed. This setup includes an initialization script that prepares the database for vector storage, making it easy to start experimenting with the notebooks provided.

To use the Docker Compose setup, ensure you have Docker and Docker Compose installed on your machine. Then, run the following command from the root of this repository:

```bash
docker-compose up -d
```

## Python Setup

To use the venv setup on Windows, ensure you have Python and venv installed on your machine. Then, follow these steps:

1. Create a virtual environment by running the following command in the root of this repository:

```bash
python.exe -m venv .venv
```

2. Activate the virtual environment by running the following command in powershell:

```bash
.\.venv\Scripts\activate
```

3. Installing the dependencies:

```bash
pip install -r requirements.txt
```

Now you are ready to use the setup with venv on Windows!
