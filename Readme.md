# Full-RAG

A FastAPI-based file upload service designed for Retrieval-Augmented Generation (RAG) applications.

## Features

- **Async file uploads** via FastAPI
- **Automatic file organization** with UUID-based naming
- **Mounted disk storage** support for large-scale document management
- **Hot reload development** server

## Project Structure
full-rag/
├── app/
│ ├── main.py
│ ├── server.py # FastAPI application with upload endpoint
│ └── utils/
│ └── file.py # Async file operations
├── run.sh # Start development server
├── freeze.sh # Generate requirements.txt
└── requirements.txt # Python dependencies


## Setup

1. Install dependencies:
```bash
pip install -r requirements.txt

2. Set up upload directory:
sudo mkdir -p /mnt/uploads
sudo chown -R $(whoami) /mnt/uploads

3. Run the server:
sh run.sh

The API will be available at http://localhost:8000

API Endpoints
GET / - Health check
POST /upload - Upload a file (returns file_id)