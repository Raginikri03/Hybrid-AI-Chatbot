# 🤖 AI Chatbot – Hybrid Chat Assistant (Groq + Ollama)
This is an intelligent hybrid chatbot built using Streamlit and LangChain that can function in both online and offline modes. It uses Groq’s hosted large language models for real-time inference and Ollama’s local models for offline capability. The chatbot also maintains conversation memory using ConversationBufferMemory for more context-aware and human-like interactions.

## Features:
Model Switching: Choose between online (Groq) or offline (Ollama) mode.

Model Options:

Groq: mixtral-8x7b-32768, llama3-8b, gemma-7b

Ollama: gemma2:2b, llama3.2, mistral

Conversation Memory: Uses LangChain's memory to retain chat history for context-aware replies.

Sidebar Configuration: Easily switch models and modes via sidebar controls.

Clear Chat Option: Reset the session with a single click.

Dynamic Prompting: Uses LangChain's ChatPromptTemplate to structure conversation flow.

## Tech Stack:
Frontend: Streamlit

LLMs:

ChatGroq for cloud-based models

Ollama for running models locally

LangChain: For chaining prompts and memory management

Dotenv: For securely managing API keys

## How It Works:
User selects between online or offline mode.

The chatbot uses the selected LLM (Groq/Ollama).

A dynamic system prompt with chat history is created using LangChain.

The response is generated based on user input and previous conversation.

Chat history is preserved and displayed.

Users can clear the conversation using a dedicated button.

## Getting Started:
bash
Copy
Edit
pip install -r requirements.txt
streamlit run app.py
Make sure to:

Install and run Ollama if using offline models.

Set your GROQ_API_KEY in a .env file if using Groq.

## Example .env File
ini
Copy
Edit
GROQ_API_KEY=your_groq_api_key_here
## Use Cases:
Personal AI assistant (offline & online)

Interview practice with memory

Context-aware helpdesk simulation

Educational tool for LLM experimentation
