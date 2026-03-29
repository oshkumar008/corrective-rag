# Corrective RAG (Retrieval-Augmented Generation)

A comprehensive implementation of Corrective Retrieval-Augmented Generation (CRAG) techniques for improving the quality and accuracy of language model responses through intelligent document retrieval and refinement.

## Project Overview

This project demonstrates various approaches to building robust RAG systems with corrective mechanisms. It includes implementations ranging from basic RAG to advanced techniques like:
- Basic RAG pipelines
- Retrieval refinement strategies
- Retrieval evaluation and validation
- Web search integration for fallback mechanisms
- Query rewriting for improved retrieval
- Handling ambiguous queries

## Project Structure

```
My-correct-rag/
├── 1_basic_rag.ipynb                    # Introduction to basic RAG concepts
├── 2_retrieval_refinement.ipynb         # Techniques to improve retrieval quality
├── 3_retrieval_evaluator.ipynb          # Methods to evaluate retrieval performance
├── 4_web_search_refinement.ipynb        # Integration of web search for enhanced results
├── 5_query_rewrite.ipynb                # Query transformation and rewriting strategies
├── 6_ambiguous.ipynb                    # Handling ambiguous and complex queries
├── requirements.txt                      # Project dependencies
├── .gitignore                           # Git ignore rules
├── documents/                           # Reference documents
│   ├── book1.pdf
│   ├── book2.pdf
│   ├── book3.pdf
│   └── readme.md
└── README.md                            # This file
```

## Notebooks Description

### 1. Basic RAG (`1_basic_rag.ipynb`)
Introduces fundamental RAG concepts including document retrieval, embedding generation, and response generation using retrieved context.

### 2. Retrieval Refinement (`2_retrieval_refinement.ipynb`)
Explores techniques to improve the quality of retrieved documents, including re-ranking and filtering strategies.

### 3. Retrieval Evaluator (`3_retrieval_evaluator.ipynb`)
Implements evaluation metrics to assess the quality and relevance of retrieved documents.

### 4. Web Search Refinement (`4_web_search_refinement.ipynb`)
Integrates web search capabilities as a fallback mechanism when document search yields insufficient results.

### 5. Query Rewrite (`5_query_rewrite.ipynb`)
Demonstrates query transformation techniques to improve retrieval results through semantic reformulation.

### 6. Ambiguous Queries (`6_ambiguous.ipynb`)
Addresses challenges in handling ambiguous or complex user queries with clarification and disambiguation strategies.

## Setup Instructions

### Prerequisites
- Python 3.8 or higher
- pip package manager
- Virtual environment (recommended)

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/oshkumar008/corrective-rag.git
   cd My-correct-rag
   ```

2. **Create and activate a virtual environment**
   ```bash
   # On Windows
   python -m venv venv
   venv\Scripts\activate
   
   # On macOS/Linux
   python -m venv venv
   source venv/bin/activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## Usage

### Running Notebooks

1. Install Jupyter (if not included in requirements.txt)
   ```bash
   pip install jupyter
   ```

2. Start Jupyter Notebook
   ```bash
   jupyter notebook
   ```

3. Open and run the notebooks in order (1-6) for the recommended learning progression

### Key Modules

Ensure the following are installed (check `requirements.txt`):
- `langchain` - Core RAG framework
- `openai` or similar LLM provider APIs
- `faiss` or `pinecone` - Vector database for embeddings
- `pandas` - Data manipulation
- `numpy` - Numerical operations

## Configuration

Before running the notebooks, configure your API keys and settings:

1. Create a `.env` file in the project root
   ```env
   OPENAI_API_KEY=your_api_key_here
   # Add other required API keys
   ```

2. Update configuration in individual notebooks as needed

## Getting Started

1. Start with `1_basic_rag.ipynb` to understand RAG fundamentals
2. Progress through notebooks 2-6 to explore advanced techniques
3. Experiment with parameters and techniques in your own notebooks
4. Reference the documents in the `documents/` folder for context

## Dependencies

All required packages are listed in `requirements.txt`. Key dependencies include:
- LangChain for RAG orchestration
- Vector databases for efficient retrieval
- LLM APIs (OpenAI, etc.)
- Document processing libraries

Run `pip install -r requirements.txt` to install all dependencies.

## Contributing

Contributions are welcome! Please feel free to:
- Report issues and bugs
- Suggest improvements
- Submit pull requests with enhancements

## License

This project is licensed under the MIT License - see LICENSE file for details.

## References

- [LangChain Documentation](https://python.langchain.com/)
- [RAG Survey Papers](https://arxiv.org/)
- [Vector Databases](https://www.pinecone.io/) and [FAISS](https://github.com/facebookresearch/faiss)

## Contact

For questions or support, please reach out to [oshkumar008](https://github.com/oshkumar008)

---

**Last Updated:** March 2026
