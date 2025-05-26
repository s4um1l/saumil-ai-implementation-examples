# Advanced Graph RAG: Investment Intelligence

An implementation example demonstrating how to build a sophisticated Retrieval-Augmented Generation (RAG) system using knowledge graphs for investment intelligence.

## 📝 Description

This example showcases how to leverage Neo4j graph database and LangChain to create a powerful RAG system for investment analysis. The implementation demonstrates:

- Building and querying knowledge graphs for investment data
- Integrating graph-based retrieval with LLMs
- Visualizing investment relationships and insights
- Advanced RAG techniques for investment intelligence

## 🔗 Resources

- Blog Post: [Coming Soon]()
- Video Tutorial: [Coming Soon]()

## 🛠️ Setup Instructions

### Prerequisites

#### Neo4j Database Setup

This project uses Neo4j's managed database service (Neo4j Aura) instead of a local installation. You'll need to:

1. Create a free Neo4j Aura account at [Neo4j Aura](https://neo4j.com/cloud/platform/aura-graph-database/)
2. Create a new instance of Neo4j Aura
3. Save your database credentials (URI, username, and password) for use in the application

The connection details will be used in the notebook to connect to your Neo4j database.

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
cd saumil-ai-implementation-examples/graph-rag

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

- [Graph RAG Implementation](./graph.ipynb): Demonstrates the complete implementation of the Graph RAG system for investment intelligence.

## 📄 License

MIT License - See the main repository LICENSE file for details.

## 📬 Contact

For questions or feedback about this example, please contact:

Saumil Srivastava  
AI Engineering Consultant  
[Contact](https://www.saumilsrivastava.ai/book-consultation) 