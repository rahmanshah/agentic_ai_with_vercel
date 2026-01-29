# Agentic AI with Vercel

This project serves as a foundation for building Agentic AI applications using Python and FastAPI, optimized for serverless deployment on Vercel.

## Features

- **FastAPI Framework**: A modern, fast (high-performance) web framework for building APIs with Python.
- **Vercel Deployment**: Pre-configured for seamless deployment to Vercel's serverless platform.
- **Python 3.12+**: Leverages the latest features of Python.

## Getting Started

### Prerequisites

- Python 3.12 or higher
- Node.js and npm (required for Vercel CLI)
- [Vercel CLI](https://vercel.com/docs/cli) (optional, for deployment)

### Setup

1. **Clone the repository:**
   ```bash
   git clone <your-repo-url>
   cd agentic_ai_with_vercel
   ```

2. **Create and activate a virtual environment:**
   ```bash
   python -m venv .venv
   
   # Windows
   .venv\Scripts\activate

   # macOS/Linux
   source .venv/bin/activate
   ```

3. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

## Running Locally

Start the development server using Uvicorn:

```bash
uvicorn instant:app --reload
```

Open your browser and navigate to `http://localhost:8000`. You should see the message: `"Live from production!"`.

## Deployment on Vercel

1. Make sure you have the [Vercel CLI](https://vercel.com/docs/cli) installed:
   ```bash
   npm install -g vercel
   ```

2. Deploy the application:
   ```bash
   vercel login
   vercel .
   ```

## Project Structure

- `instant.py`: The entry point for the FastAPI application.
- `requirements.txt`: Lists the Python dependencies.
- `vercel.json`: Configuration file for Vercel deployment.
