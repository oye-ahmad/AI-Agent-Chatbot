## 🤖 AI Agent Chatbot ##
Smart, Tool-Enabled Conversational AI using FastAPI, LangGraph & Streamlit

An intelligent, customizable AI Agent that dynamically selects large language models (Groq / OpenAI), supports real-time web search, and provides a clean interactive UI for human-AI conversations.

## 🌟 Project Overview

This project implements a tool-augmented AI Agent chatbot using LangGraph’s ReAct agent architecture. The system allows users to:

--> Define custom AI personalities (system prompts)

--> Choose between Groq and OpenAI models

--> Enable or disable real-time web search

--> Interact via a Streamlit-based UI

--> Communicate securely through a FastAPI backend

The architecture cleanly separates UI, API, and AI reasoning logic, making the project modular, scalable, and production-ready.

## Key Features

🧠 ReAct-based AI Agent using LangGraph

🔁 Dynamic LLM Selection

Groq (LLaMA, Mixtral)

OpenAI (GPT-4o-mini)

🔍 Optional Web Search Integration

Powered by Tavily Search API

🖥️ Interactive Streamlit Frontend

⚡ FastAPI Backend with Validation

🧩 Modular & Extensible Design

🔐 Secure API Key Management via Environment Variables

## How the AI Agent Works

User defines an AI role (system prompt)

User selects:

Model provider (Groq / OpenAI)

Model name

Web search permission

Frontend sends request to FastAPI

Backend validates the request

LangGraph creates a ReAct agent

Agent:

Thinks

Decides whether to search

Generates a final response

Response is sent back to UI

## Project Architecture

📦 AI-Agent-Chatbot
 
 ┣ 📜 ai_agent.py      # Core AI agent logic (LangGraph + tools)
 
 ┣ 📜 backend.py       # FastAPI backend and API endpoint
 
 ┣ 📜 frontend.py      # Streamlit-based user interface
 
 ┣ 📜 README.md        # Project documentation
 
 ┣ 📜 requirements.txt # Python dependencies
 
 ┗ 📜 .gitignore       # Ignored files (env, cache, etc.)

 ## Technologies Used

-- Python 3.10+

-- FastAPI – Backend API

-- Streamlit – Frontend UI

-- LangChain & LangGraph – AI agent orchestration

-- Groq API – High-performance LLM inference

-- OpenAI API – GPT-4o-mini

-- Tavily Search API – Web search tool

-- Uvicorn – ASGI server

## How to Run the Project

1️⃣ Install Dependencies

pip install -r requirements.txt

2️⃣ Start the FastAPI Backend

python backend.py

Swagger Docs:
  http://127.0.0.1:9999/docs

3️⃣ Start the Streamlit Frontend

streamlit run frontend.py

## 🔮 Future Enhancements

Conversation memory (multi-turn chat)

Authentication & user sessions

Deployment on Docker / Cloud

Tool chaining (PDFs, files, code execution)

UI enhancements with chat history

## 👨‍💻 Author

Ahmad

Undergraduate Computer Engineering Student

UET Taxila

Passionate about AI/ML, Data Science, App Development and Bug Hunting

## ⭐ Acknowledgements

--> LangChain & LangGraph Team

--> Groq AI

--> OpenAI

--> Tavily Search
