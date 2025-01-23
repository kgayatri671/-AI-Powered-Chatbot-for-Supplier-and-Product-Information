# -AI-Powered-Chatbot-for-Supplier-and-Product-Information

# AI-Powered Chatbot for Supplier and Product Information

Overview
This project implements an AI-powered chatbot that allows users to query supplier and product information using natural language. The chatbot integrates an open-source LLM for summarizing supplier information and uses the LangGraph framework for agent workflows. The backend is built with FastAPI, while the frontend uses React for a responsive and user-friendly UI.

The system interacts with a MySQL/PostgreSQL database to fetch and provide relevant details about products and suppliers.

Tech Stack
Backend
Framework: FastAPI
LLM Workflow: LangGraph
Database: MySQL/PostgreSQL
Language: Python
Frontend
Framework: React
Styling: Material UI or Tailwind CSS
State Management: Redux or Context API
API Calls: Axios
Database
MySQL/PostgreSQL for storing product and supplier information.
System Architecture
The project is organized into the following components:

Frontend: React-based interface to input queries and display chatbot responses.
Backend: FastAPI server that processes user queries, fetches data from the database, and enhances responses using an LLM.
Database: Stores structured data about products and suppliers.
LLM: Summarizes data and provides natural language enhancements for chatbot responses.



## Features

- Query products and suppliers via chatbot.
- Summarize supplier data using an LLM.
- Conversational UI for interaction.
- Features
Natural Language Queries: Users can query products and suppliers using conversational text.
Database Integration: The chatbot retrieves data from a structured MySQL/PostgreSQL database.
AI Summarization: Uses a language model (e.g., GPT-2, GPT-3, or LLAMA 2) to summarize supplier data.
Frontend: A responsive and interactive UI built with React.
Error Handling: Handles invalid or incomplete queries gracefully.


## Installation

### Backend
1. Navigate to the `backend` folder:
   ```bash
   cd backend
Usage

Interact with the chatbot by entering queries like:
"Show me all products under brand X."
"Which suppliers provide laptops


CREATE TABLE Products (
    id SERIAL PRIMARY KEY,
    name VARCHAR(100),
    brand VARCHAR(50),
    price DECIMAL(10, 2),
    category VARCHAR(50),
    description TEXT,
    supplier_id INT
);

CREATE TABLE Suppliers (
    id SERIAL PRIMARY KEY,
    name VARCHAR(100),
    contact_info TEXT,
    product_categories TEXT
);
Project Folder Structure
AI-Powered-Chatbot/
├── backend/
│   ├── app/
│   │   ├── __init__.py
│   │   ├── main.py
│   │   ├── database.py
│   │   ├── models.py
│   │   ├── routes.py
│   │   ├── langgraph_workflow.py
│   └── requirements.txt
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   │   ├── ChatBox.js
│   │   │   └── QueryHistory.js
│   │   ├── App.js
│   │   ├── index.js
│   └── package.json
├── README.md
└── .gitignore
