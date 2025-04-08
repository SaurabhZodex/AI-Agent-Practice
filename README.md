# AI Agent Practice Repository

Practice implementation of multi-agent AI systems using Autogen, Langchain, LangGraph, and CrewAI. Features three specialized agents with memory capabilities for book analysis, weather data, and internet search.

## 📌 Overview
This repository contains an experimental setup for creating AI agent systems that can:
- Answer questions about specific books using vector databases
- Fetch real-time weather information
- Perform internet searches
- Maintain conversation memory and context

Frameworks used:
- **Autogen**: Multi-agent conversations
- **Langchain**: Vector DB/book analysis
- **LangGraph**: Agent workflow orchestration
- **CrewAI**: Task delegation and coordination

## 🚀 Features

### 📚 Book Analysis Agent
- Vector DB for "Verity" & "The Girl on the Train"
- Uses Chroma + BAAI/llm-embedder embeddings
- Long-term memory for conversation history

### 🔍 Internet Search Agent
- Serper API integration (Google Search)
- Summary generation from results
- Search history tracking

## ⚙️ Installation

1. Clone repo:
```bash
git clone https://github.com/SaurabhZodex/AI-Agent-Practice.git
cd AI-Agent-Practice
```

2. Create virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # Linux/Mac
venv\Scripts\activate  # Windows
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## 📂 Project Structure
```
|── README.md
├── autogen_agents.ipynb       # Autogen implementations
├── langchain_agents.ipynb     # Langchain implementations
├── langgraph_agents.ipynb     # LangGraph workflows
├── crewai_agents.ipynb        # CrewAI task orchestration
├── Dataset/                   # Book texts
├── requirements.txt           # Python dependencies
└── .env                       # Environment variables
```

## 🔍 Framework Comparison Guide

| Criteria         | Langchain | Autogen | LangGraph | CrewAI |
|------------------|-----------|---------|-----------|--------|
| Ease of Use      | ★★★★☆     | ★★★☆☆   | ★★☆☆☆     | ★★★★☆  |
| Memory Handling  | ★★★★☆     | ★★★☆☆   | ★★★★☆     | ★★★☆☆  |
| Agent Complexity | ★★☆☆☆     | ★★★★☆   | ★★★★★     | ★★★☆☆  |
| API Integration  | ★★★★★     | ★★★★☆   | ★★★☆☆     | ★★★★☆  |