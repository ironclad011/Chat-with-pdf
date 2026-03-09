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
│   ├── main.py
│   ├── server.py
│   └── utils/
│       └── file.py
├── run.sh
├── freeze.sh
└── requirements.txt


## Setup

1. Install dependencies:

Bash
pip install -r requirements.txt

2. Set up upload directory:

Bash
sudo mkdir -p /mnt/uploads
sudo chown -R $(whoami) /mnt/uploads

3. Run the server:

Bash
sh run.sh
The API will be available at: http://localhost:8000
