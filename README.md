# Flask App with Milvus and DistilBert

This Flask application demonstrates how to use Milvus as a vector database and DistilBert from Hugging Face's Transformers library to create and search for text embeddings.

## Prerequisites

- Python 3.8 or newer
- Docker (for running Milvus)
- An environment where Flask can be run

## Setup

### 1. Install Dependencies

First, install the required Python libraries:

```bash
pip install flask pymilvus transformers torch milvus

### 1. Start Milvus

milvus-server

### 1. In a new tab or session, run the applicaiton.

python search-api.py

### 1. Sample Request:

curl -X POST http://localhost:5000/search -H "Content-Type: application/json" -d '{"query": "your search text here"}'
