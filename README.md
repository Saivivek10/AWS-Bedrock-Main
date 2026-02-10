# AWS-Bedrock PDF Chat Application

This project is a Streamlit-based application that allows users to interact with PDF documents using AWS Bedrock's generative AI models. The application supports querying PDF content and generating responses using advanced language models like Claude and Llama2.

## Features

- **PDF Data Ingestion**: Load and process PDF files to extract text for querying.
- **Vector Embedding**: Generate embeddings using Amazon Titan Embeddings and store them in a FAISS vector database.
- **Query Answering**: Use generative AI models (Claude and Llama2) to answer user queries based on the PDF content.
- **Interactive UI**: A user-friendly Streamlit interface for uploading PDFs, updating vector stores, and querying data.

## How It Works

1. **Data Ingestion**: The application reads PDF files from the `data/` directory and splits the text into chunks for processing.
2. **Vector Store Creation**: The text chunks are converted into embeddings using Amazon Titan Embeddings and stored in a FAISS index.
3. **Query Processing**: User queries are matched with the most relevant text chunks using the FAISS index, and the selected generative AI model generates a detailed response.

## Requirements

- Python 3.8+
- AWS credentials configured for accessing Bedrock services
- Required Python libraries (see `requirements.txt`)

## Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd AWS-Bedrock
