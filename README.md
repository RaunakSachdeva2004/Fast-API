# FastAPI Application

A lightweight RESTful API service built with FastAPI and Uvicorn. This repository provides a starter implementation demonstrating routing, request handling, and automated API documentation.

## Features

- High-performance asynchronous API framework powered by Starlette and Pydantic.
- Automatic interactive API documentation via Swagger UI and ReDoc.
- Minimal and clean project structure for rapid development.

## Prerequisites

- Python 3.10 or higher
- pip (Python package installer)

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/RaunakSachdeva2004/Fast-API.git
   cd Fast-API
   ```

2. Create and activate a virtual environment:
   - On Windows (PowerShell):
     ```powershell
     python -m venv myvenv
     .\myvenv\Scripts\Activate.ps1
     ```
   - On macOS/Linux:
     ```bash
     python3 -m venv myvenv
     source myvenv/bin/activate
     ```

3. Install required dependencies:
   ```bash
   pip install fastapi uvicorn
   ```

## Usage

Start the development server using Uvicorn with auto-reload enabled:

```bash
uvicorn main:app --reload
```

The server will be available at `http://127.0.0.1:8000`.

## API Endpoints

### Root Endpoint
- Method: `GET`
- Path: `/`
- Description: Returns a welcome JSON response.
- Response:
  ```json
  {
    "message": "hello world"
  }
  ```

## Interactive Documentation

FastAPI automatically generates interactive API documentation. When the application is running, navigate to:
- Swagger UI: `http://127.0.0.1:8000/docs`
- ReDoc: `http://127.0.0.1:8000/redoc`

## Project Structure

```text
Fast-API/
|-- main.py          # Application entry point and route definitions
|-- .gitignore       # Git ignore configuration
|-- LICENSE          # MIT License
|-- README.md        # Project documentation
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.