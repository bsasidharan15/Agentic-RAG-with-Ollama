# Agentic-RAG-with-Ollama

This project implements a Retrieval-Augmented Generation (RAG) pipeline using LangChain, FAISS, and Ollama's llama3 embeddings to enable intelligent, agent-based question-answering over a custom document. It includes a simple agentic setup that processes and answers questions about a medical report.

🚀 Features
Loads and parses a custom document.

Splits content into manageable chunks for embedding.

Generates vector embeddings using Ollama's LLaMA3 model.

Stores embeddings using FAISS vector store.

Implements a LangChain agent capable of querying the document contextually.

Includes a basic tool wrapper and agent prompt for enhanced response accuracy.

🧠 Technologies Used
LangChain

Ollama

FAISS

Python

Jupyter Notebook

📁 Project Structure
python
Copy
Edit
Agentic-RAG-with-Ollama/
├── agents.ipynb                # Jupyter notebook containing the complete pipeline
├── requirements.txt            # (Optional) Dependencies list
└── README.md                   # You're reading it!
📄 Setup Instructions
Install dependencies

bash
Copy
Edit
pip install langchain langchain-community langchain-ollama faiss-cpu tiktoken
Prepare your knowledge base

Replace the path in this line of the notebook:

python
Copy
Edit
TextLoader("path/to/your/document.txt")
Run the notebook

Launch the notebook and run all cells sequentially to:

Load and preprocess the document

Generate and store embeddings

Initialize the agent

Query the document interactively

💡 Example Use Case
Ask the agent:

"What symptoms did Michael Johnson experience?"

And receive a contextual response based on the contents of the medical report provided.

🛠️ Notes
Ensure ollama is properly set up and the llama3 model is available locally.

For large documents, consider tuning chunk_size and chunk_overlap.
