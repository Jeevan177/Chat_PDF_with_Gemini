# Chat_PDF_with_Gemini

This project allows users to interact with PDF documents by asking questions and receiving AI-generated responses. It leverages Google Gemini's Generative AI and FAISS for vector-based retrieval, enabling efficient information extraction from uploaded PDFs.

## Project Overview

This application processes PDFs, extracts text, and enables question-answering through embeddings and conversational AI. It follows these key steps:

1. **Upload PDF Files**: Users can upload multiple PDF documents.
2. **Extract Text**: The text is extracted from PDFs using PyPDF2.
3. **Split Text into Chunks**: Large texts are divided into manageable chunks using RecursiveCharacterTextSplitter.
4. **Generate Embeddings**: The extracted text chunks are converted into vector embeddings using GoogleGenerativeAIEmbeddings.
5. **Store in FAISS**: The embeddings are stored in a FAISS vector database for fast similarity searches.
6. **Process User Queries**: Users enter queries, and the system retrieves relevant chunks from FAISS.
7. **Generate Responses**: A chatbot powered by ChatGoogleGenerativeAI provides detailed responses based on the retrieved context.

## Technologies Used:
- **Streamlit**:  For building the web interface
- **PyPDF2**: For extracting text from PDFs
- **LangChain**: For managing text processing and embeddings
- **Google Generative AI (Gemini)**: For embeddings and AI-driven responses
- **FAISS**: For storing and searching text embeddings
- **dotenv**: For managing API keys securely

## Installation & Setup:

1. Clone the Repository
2. Create and Activate Virtual Environment
3. Install the required Python libraries (`pip install -r requirements.txt`).
4. Set Up API Key Create a .env file in the root directory and add your Google API key:
5. Run the application

## How to Use:

1. Upload PDF Files in the sidebar.
2. Click "Submit & Process" to extract text and store it in FAISS.
3. Ask Questions in the input field.
4. The AI will retrieve relevant information and provide a response.   
