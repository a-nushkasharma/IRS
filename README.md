# Information-Retrieval-System

IRS is a PDF-based question-answering application built with Streamlit and LangChain. It allows users to upload PDF documents (size limit:200MB) and ask natural language questions based on the context of the source PDF. The system returns relevant answers extracted from the uploaded content using semantic search and LLM-powered contextual understanding.

🔍 Features

Upload multiple PDF files

Extract and process text using PyPDF2

Chunk text data for efficient retrieval

Generate vector embeddings using LLM models

Semantic search via FAISS vector store

Interactive chatbot UI to ask questions about uploaded content

Conversational memory with context-aware answers

🛠️ Tech Stack

Frontend/UI: Streamlit

Backend/Processing: Python, LangChain

Text Parsing: PyPDF2

Text Embedding & LLM: Hugging Face models (or OpenAI/Gemini if preferred)

Vector Store: FAISS

Environment Management: Python-dotenv

🧪 Installation

1. Clone the Repository
```bash
Copy
Edit
git clone https://github.com/yourusername/irs-project.git
cd irs-project
```
2. Create a Virtual Environment
```bash
Copy
Edit
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```
3. Install Requirements
```bash
Copy
Edit
pip install -r requirements.txt
```
4. Set Environment Variables
Create a .env file in the project root and add your API key if using a provider like OpenAI or Hugging Face:
```bash
ini
Copy
Edit
OPENAI_API_KEY=your_openai_key
HUGGINGFACEHUB_API_TOKEN=your_huggingface_token
```
5. Run the Application
```bash
Copy
Edit
streamlit run app.py
Access the app in your browser at http://localhost:8501.
```

📁 Project Structure
```bash 
IRS/ 

├── app.py                  # Main application file

├── requirements.txt        # Python dependencies

├── README.md               # Project documentation

├── .env                    # Environment variables (not pushed to GitHub)

├── src/                    # Source folder

│   └── helper.py           # Helper functions (text extraction, chunking, etc.)

├── data/                   # Folder to hold uploaded or test PDFs

│   └── sample.pdf

└── assets/                 # Optional static assets like logos
    └── logo.png
```
💬 Usage

Upload PDF files in the sidebar.

Wait for the system to extract and embed content.

Type your question in the input box.

View answers and chat history in the main window.

🙋‍♀️ Contributions
Pull requests and issue reports are welcome. Please fork the repository and submit your changes via PR.
