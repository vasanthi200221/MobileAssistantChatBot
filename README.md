# MobileAssistantChatBot
This project is an AI-powered chatbot that fetches and displays the latest phone models in real time. It integrates an external mock API and utilizes Ollama (an open-source alternative to OpenAI) for natural language processing.

🚀 Features

Fetches the latest phone models from a mock API.

Uses Ollama (Mistral model) for AI-driven phone recommendations.

Interactive chatbot for users to ask phone-related queries.

Web UI powered by Gradio.

FastAPI backend for API integration.

🛠 Installation Guide

1️⃣ Install Anaconda & Jupyter Notebook

If you haven't installed Anaconda yet, download and install it from:
👉 Anaconda Official Site

After installation, open Anaconda Prompt and run:

conda install -c conda-forge jupyterlab

2️⃣ Install Required Python Packages

Create a new environment (optional but recommended):

conda create --name phonebot python=3.10 -y
conda activate phonebot

Now, install the required dependencies:

pip install fastapi uvicorn gradio requests nest_asyncio ollama

3️⃣ Install Ollama (Windows)

Ollama is an open-source alternative to OpenAI, providing free, local AI processing.

✅ Install Ollama on Windows:

Download the installer from 👉 https://ollama.com

Run the installer and follow the on-screen instructions.

Verify installation by running:

ollama --help

Pull the Mistral model (used for AI chatbot processing):

ollama pull mistral

🏃‍♂️ Running the Project

1️⃣ Start the Mock API

Before running the chatbot, start the mock API:

Open Jupyter Notebook.

Run mockapi.ipynb to start the API.

This API serves the latest phone models at http://127.0.0.1:8000/latest.

Note: mockapi.ipynb must remain running until the PhoneAssistanceChatBot.ipynbt is in use.

2️⃣ Start the Chatbot

Open PhoneAssistanceChatBot.ipynb in Jupyter Notebook.

Run all cells.

This will:

Start a FastAPI server on http://127.0.0.1:8003.

Launch a Gradio web UI on http://127.0.0.1:7861.

Interact with the chatbot by typing queries!

❓ Why Use Ollama Instead of OpenAI?

Open-source: No API keys or paid subscriptions required.

Runs locally: No internet dependency, fast and secure.

Completely free: Unlike OpenAI, no cost is incurred!

🔧 Troubleshooting

Error: [Errno 10048] error while attempting to bind on address ('127.0.0.1', 8003)

🔹 Solution: A process is already using port 8003. Either:

Close any existing FastAPI servers (CTRL+C in the terminal).

Change the port in the script (e.g., 8004 instead of 8003).

📝 Summary

This project leverages FastAPI, Gradio, and Ollama to create an AI-driven phone chatbot. Follow the installation and setup steps carefully to get started. 🚀

🔹 Developed by:Vasanthi Mopuru

