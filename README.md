# Advance RAG - Chat with Your Files

This project is a Retrieval-Augmented Generation (RAG) application built with Streamlit and LangChain. It allows you to upload documents (PDF, CSV, TXT), process them, and interact with them using conversational AI powered by Google Gemini.

## Features

- Upload PDF, CSV, and TXT files
- Chunk and embed documents using Sentence Transformers
- Store and retrieve document embeddings with Chroma
- Ask questions and get answers based on your uploaded files
- Conversation history saved for reference

## Getting Started

### Prerequisites

- Python 3.8+
- [pip](https://pip.pypa.io/en/stable/)
- Google Gemini API key (set in `.env` file)

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/advance-rag.git
    cd advance-rag
    ```

2. Install dependencies:
    ```sh
    pip install -r requirements.txt
    ```

3. Create a `.env` file and add your Google API key:
    ```
    GOOGLE_API_KEY=your_google_gemini_api_key
    ```

### Usage

Run the Streamlit app:

```sh
streamlit run ui.py
```

Open your browser and go to the URL shown in the terminal.

### File Upload

- Use the sidebar to upload PDF, CSV, or TXT files.
- Adjust chunk size and overlap as needed.

### Ask Questions

- Type your question in the chat box.
- The app retrieves relevant document chunks and generates an answer using Gemini.

## Project Structure

- `ui.py` - Streamlit user interface
- `rag_utils.py` - Core logic for file processing, embedding, retrieval, and QA
- `vector_store/` - Stores vector database and conversation history
- `.env` - Environment variables (not tracked by git)
- `.gitignore` - Files and folders to ignore in git

## License

MIT License

## Acknowledgements

- [LangChain](https://github.com/langchain-ai/langchain)
- [Streamlit](https://streamlit.io/)
- [Chroma](https://www.trychroma.com/)
- [Google Gemini](https://ai.google.dev/gemini-api/docs/)
