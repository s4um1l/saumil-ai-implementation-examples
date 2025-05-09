# Metadata Filtering in Vector Search

A comprehensive implementation guide demonstrating metadata filtering capabilities across different vector databases (Milvus, Qdrant, Pinecone, Weaviate), providing practical examples and performance considerations for engineering teams.

## 📝 Description

This repository contains practical examples of metadata filtering in vector databases, showcasing how to:

- Filter vector search results using structured metadata
- Compare different vector database approaches to metadata filtering
- Implement various filtering strategies with nested data
- Optimize performance with proper indexing techniques

## 🔗 Resources

- Blog Post: [Coming Soon]()
- Video Tutorial: [Coming Soon]()

## 🛠️ Setup Instructions

### Prerequisites

#### Docker (for Qdrant and Weaviate examples)

Docker is required to run the Qdrant and Weaviate servers locally.

##### macOS/Windows
Install [Docker Desktop](https://www.docker.com/products/docker-desktop/)

##### Ubuntu/Debian
```bash
sudo apt-get update
sudo apt-get install docker.io
```

#### API Keys (for Pinecone example)

You'll need a Pinecone API key to run the Pinecone example. Sign up for a free account at [Pinecone](https://www.pinecone.io/).

### Python Environment Setup

This project uses [uv](https://github.com/astral-sh/uv) for Python package management.

#### Install uv (if not already installed)
```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

#### Clone and setup the repository
```bash
# Clone the main repository
git clone https://github.com/saumilsrivastava/saumil-ai-implementation-examples.git
cd saumil-ai-implementation-examples/metadata-filtering

# Create a virtual environment
uv venv

# Activate the virtual environment
# On macOS/Linux:
source .venv/bin/activate
# On Windows:
# .venv\Scripts\activate

# Install dependencies
uv sync
```

## 📊 Notebooks

The implementation includes the following Jupyter notebooks:

- [Pinecone Metadata Filtering](./01_pinecone_metadata_filtering.ipynb): Explores Pinecone's metadata filtering capabilities, including namespace management, structured queries, and performance optimizations with proper indexing.

- [Weaviate Metadata Filtering](./02_weaviate_metadata_filtering.ipynb): Demonstrates Weaviate's GraphQL-based filtering approach, working with schema definitions, and leveraging both BM25 and vector search in hybrid queries.

- [Milvus Metadata Filtering](./03_milvus_metadata_filtering.ipynb): Demonstrates metadata filtering in Milvus, including setup with Milvus Lite, defining schemas with scalar and vector fields, and performing filtered vector searches.

- [Qdrant Metadata Filtering](./04_qdrant_metadata_filtering.ipynb): Showcases Qdrant's powerful metadata filtering capabilities, handling of nested JSON payloads, and flexible query syntax with `must`, `should`, and `must_not` conditions.

## 🚀 Running the Examples

### Pinecone Example
The Pinecone example connects to Pinecone's cloud service:

```bash
# Set your Pinecone API key as an environment variable
export PINECONE_API_KEY=your_pinecone_api_key

# Run the notebook
jupyter notebook 01_pinecone_metadata_filtering.ipynb
```

### Weaviate Example
The Weaviate example requires a running Weaviate instance:

```bash
# Start Weaviate server with Docker
docker run -d --name weaviate-demo \
    -p 8080:8080 \
    -e AUTHENTICATION_ANONYMOUS_ACCESS_ENABLED=true \
    -e PERSISTENCE_DATA_PATH="/var/lib/weaviate" \
    semitechnologies/weaviate:1.19.6

# Run the notebook
jupyter notebook 02_weaviate_metadata_filtering.ipynb
```

### Milvus Example
The Milvus example uses Milvus Lite, which runs embedded in Python:

```bash
jupyter notebook 03_milvus_metadata_filtering.ipynb
```

### Qdrant Example
The Qdrant example requires a running Qdrant instance:

```bash
# Start Qdrant server in Docker
docker run -d --name qdrant-demo \
    -p 6333:6333 \
    -p 6334:6334 \
    qdrant/qdrant:latest

# Run the notebook
jupyter notebook 04_qdrant_metadata_filtering.ipynb
```

## 📄 License

MIT License - See the main repository LICENSE file for details.

## 📬 Contact

For questions or feedback about these examples, please contact:

Saumil Srivastava  
AI Engineering Consultant  
[Contact](https://www.saumilsrivastava.ai/book-consultation)
