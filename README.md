

```markdown
# Gemma Model Document Q&A

This repository contains two Streamlit applications (`app1.py` and `app.py`) that use the Gemma model to answer questions based on the context provided in PDF documents. 

## Overview

- `app1.py`: Allows users to upload their PDF files, which are then processed to answer questions based on the content of the uploaded document.
- `app.py`: Uses preloaded PDF documents from a directory to answer questions based on their content.

## Features

- PDF document ingestion and vector embedding.
- Question answering based on document content using the Gemma model.
- Document similarity search to find relevant chunks of text.

## Requirements

- Python 3.8+
- Streamlit
- Langchain
- Langchain_groq
- Langchain_community
- Langchain_google_genai
- dotenv
- FAISS
- PyPDFLoader

## Setup

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/QA_RAG_GEMMA.git
   cd QA_RAG_GEMMA
   ```

2. **Create a virtual environment:**

   ```bash
   python -m venv venv
   source venv/bin/activate   # On Windows use `venv\Scripts\activate`
   ```

3. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables:**

   Create a `.env` file in the root directory and add your API keys:

   ```ini
   GROQ_API_KEY=your_groq_api_key
   GOOGLE_API_KEY=your_google_api_key
   ```

## Running the Applications

### Running `app1.py`

This application allows users to upload a PDF file and ask questions based on the document content.

1. **Run the Streamlit app:**

   ```bash
   streamlit run app1.py
   ```

2. **Upload a PDF file:**
   
   - Go to the provided local URL.
   - Upload your PDF document.
   - Enter your question and click on "Documents Embedding".

### Running `app.py`

This application uses preloaded PDF documents from a directory to answer questions.

1. **Ensure you have PDF files in the `./us_census` directory.**

2. **Run the Streamlit app:**

   ```bash
   streamlit run app.py
   ```

3. **Enter your question:**
   
   - Go to the provided local URL.
   - Enter your question in the text input and click on "Documents Embedding".

## Clean Up

Temporary files created during the execution of the apps are automatically cleaned up upon app termination.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request if you have any suggestions or improvements.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
```

This `README.md` provides a comprehensive overview of your applications, including setup, running instructions, and other relevant details. Feel free to adjust the repository URL and other specific details as necessary.
