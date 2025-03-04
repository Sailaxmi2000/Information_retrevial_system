# Information_retrevial_system

**Information Retrieval System**
An intelligent document question-answering system that allows users to upload PDFs and ask questions about their content. This application uses Google's Generative AI models combined with vector search to provide accurate answers based solely on the uploaded documents.
Features

**PDF Processing:** Upload and process multiple PDF files
**Semantic Search:** Identify relevant content using vector embeddings
**Conversational Interface:** Ask questions naturally about your documents
**Advanced RAG Implementation:** Retrieval Augmented Generation to provide accurate, contextual answers

**Technologies Used**

Python: Core programming language
Streamlit: Web application framework for the user interface
LangChain: Framework for building LLM-powered applications
Google Generative AI: Embeddings and language model (Gemini)
FAISS: Vector database for efficient similarity search
PyPDF2: PDF parsing and text extraction
dotenv: Environment variable management for API keys

**Setup Instructions**

Clone this repository
Create a Conda environment:
Copyconda create -n genai_env python=3.9
conda activate genai_env

**Install the required packages:**
Copypip install streamlit langchain langchain-community langchain-google-genai python-dotenv faiss-cpu PyPDF2

Create a .env file in the project root with your Google API key:
CopyGOOGLE_API_KEY=your_api_key_here

**Run the application:**
Copystreamlit run app.py


**Usage**

Upload PDF documents using the sidebar
Click "Submit & Process" to extract and analyze the content
Ask questions in the text input field
Receive answers based on the content of your documents

**Project Structure**

app.py: Main Streamlit application
src/helper.py: Core functionality for PDF processing, text chunking, and RAG implementation
.env: API key storage (not included in repository)

**Future Improvements**

Add support for more document types (DOCX, TXT, etc.)
Implement document persistence to avoid reprocessing
Add a chat history view for better conversation tracking
Enhance the UI with additional visualization options


