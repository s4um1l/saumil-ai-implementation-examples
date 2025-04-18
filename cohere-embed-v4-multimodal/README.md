# Cohere Embed v4 Multimodal

An implementation example for Cohere's Embed v4 multimodal embedding model, demonstrating how to effectively work with both text and image embeddings for practical AI applications.

## 📝 Description

This example showcases how to leverage Cohere's Embed v4 multimodal embedding model to create embeddings for text and images. The implementation demonstrates:

- Working with PDF files containing text and images

## 🔗 Resources

- Blog Post: [Coming Soon]()
- Video Tutorial: [Coming Soon]()

## 🛠️ Setup Instructions

### Prerequisites

#### Install poppler-utils

Poppler-utils is required for PDF processing in this project.

##### macOS
```bash
brew install poppler
```

##### Ubuntu/Debian
```bash
sudo apt-get install poppler-utils
```

##### Windows
Install using Chocolatey:
```bash
choco install poppler
```
Or download from [poppler for Windows](https://github.com/oschwartz10612/poppler-windows/releases)

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
cd saumil-ai-implementation-examples/cohere-embed-v4-multimodal

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

- [Experimenting with Cohere Embed v4](./notebooks/Experimenting_with_CohereEmbedv4.ipynb): Demonstrates the capabilities of Cohere's Embed v4 model and explores different use cases.



## 📄 License

MIT License - See the main repository LICENSE file for details.

## 📬 Contact

For questions or feedback about this example, please contact:

Saumil Srivastava  
AI Engineering Consultant  
[Contact](https://www.saumilsrivastava.ai/book-consultation)
