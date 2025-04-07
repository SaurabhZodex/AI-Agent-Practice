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
- Uses FAISS + OpenAI embeddings
- Long-term memory for conversation history

### 🌦️ Weather Agent
- OpenWeatherMap API integration
- Caching mechanism for frequent queries
- Location context maintenance

### 🔍 Internet Search Agent
- Serper API integration (Google Search)
- Summary generation from results
- Search history tracking

## ⚙️ Installation

1. Clone repo:
```bash
git clone https://github.com/yourusername/ai-agents-practice.git
cd ai-agents-practice
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

## 🔑 Configuration

1. Create `.env` file:
```ini
OPENAI_API_KEY=your_openai_key
OPENWEATHER_API_KEY=your_weather_key
SERPER_API_KEY=your_serper_key
```

## 📂 Project Structure
```
|── README.md
├── autogen_agents.py       # Autogen implementations
├── langchain_agents.py     # Langchain implementations
├── langgraph_agents.py     # LangGraph workflows
├── crewai_agents.py        # CrewAI task orchestration
├── data/                   # Book texts
├── requirements.txt
└── .env.example
```

## 🔍 Framework Comparison Guide

| Criteria         | Langchain | Autogen | LangGraph | CrewAI |
|------------------|-----------|---------|-----------|--------|
| Ease of Use      | ★★★★☆     | ★★★☆☆   | ★★☆☆☆     | ★★★★☆  |
| Memory Handling  | ★★★★☆     | ★★★☆☆   | ★★★★☆     | ★★★☆☆  |
| Agent Complexity | ★★☆☆☆     | ★★★★☆   | ★★★★★     | ★★★☆☆  |
| API Integration  | ★★★★★     | ★★★★☆   | ★★★☆☆     | ★★★★☆  |