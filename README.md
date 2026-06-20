# IIT Kanpur Information Assistant

A Retrieval-Augmented Generation (RAG) chatbot that answers questions related to IIT Kanpur using information collected from official institute resources.

## Features

- Semantic search using vector embeddings
- Context-aware question answering
- Streamlit-based web interface
- Google Gemini for response generation
- ChromaDB for document retrieval

## Tech Stack

- Python
- Streamlit
- LangChain
- ChromaDB
- Google Gemini API
- pyngrok

## Setup

### 1. Clone the Repository

bash git clone <repository-url> cd <repository-name> 

### 2. Install Dependencies

bash pip install -r requirements.txt 

### 3. Add Your Credentials

Replace the placeholders in the notebook/code:

python os.environ["GOOGLE_API_KEY"] = "YOUR_API_KEY_HERE" 

python ngrok.set_auth_token("YOUR_NGROK_AUTH_TOKEN") 

## Running the Project

Launch the Streamlit app:

bash streamlit run app.py 

If using Google Colab, run the ngrok cell to generate a public URL for the application.

## How It Works

1. Documents are collected and processed.
2. Text embeddings are generated and stored in ChromaDB.
3. Relevant information is retrieved for each query.
4. Gemini generates responses using the retrieved context.

## Notes

- Do not upload personal API keys or ngrok tokens to GitHub.
- Generate your own Google API key and ngrok token before running the project.

## Author

Prajit Vaman T S  
Department of Mathematics and Statistics  
IIT Kanpur
