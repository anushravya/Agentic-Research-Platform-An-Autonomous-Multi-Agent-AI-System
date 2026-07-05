
# Agentic Research Platform: An Autonomous Multi-Agent AI System

## Overview

Agentic Research Platform is an AI-powered application that automates the research process using multiple intelligent agents. The platform performs web search, extracts relevant information from websites, and generates concise summaries using Large Language Models (LLMs).

The system follows an autonomous multi-agent architecture where specialized agents collaborate to retrieve, analyze, and summarize information efficiently.

---

## Features

- Autonomous Multi-Agent Architecture
- Intelligent Web Search using Tavily Search API
- Web Scraping using BeautifulSoup
- ReAct Agent Reasoning
- LangChain LCEL Runnable Pipeline
- AI-powered Research Summarization
- Environment Variable Management with `.env`
- Modular and Scalable Project Structure

---

## Tech Stack

- Python
- OpenAI GPT
- LangChain (LCEL)
- Tavily Search API
- BeautifulSoup4
- Requests
- Python Dotenv
- UV Package Manager

---

## Project Architecture

```
User Query
      │
      ▼
Research Agent
      │
      ▼
Tavily Search API
      │
      ▼
Website URLs
      │
      ▼
BeautifulSoup Web Scraper
      │
      ▼
Extracted Content
      │
      ▼
Summarization Agent
      │
      ▼
Final Research Report
```

---

## Project Structure

```
agentic-research-platform/
│
├── agents/
│   ├── researcher.py
│   └── summarizer.py
│
├── tools/
│   ├── tavily_tool.py
│   └── scraper.py
│
├── prompts/
│
├── pipeline/
│
├── utils/
│
├── main.py
├── pyproject.toml
├── uv.lock
├── .env.example
├── README.md
└── .gitignore
```

---

## Installation

### Clone the repository

```bash
git clone https://github.com/anushravya/agentic-research-platform.git

cd agentic-research-platform
```

### Create a Virtual Environment

```bash
uv venv
```

Activate it

Windows

```bash
.venv\Scripts\activate
```

Linux / macOS

```bash
source .venv/bin/activate
```

---

## Install Dependencies

```bash
uv sync
```

or

```bash
uv pip install -r requirements.txt
```

---

## Environment Variables

Create a `.env` file.

```env
OPENAI_API_KEY=your_openai_api_key

TAVILY_API_KEY=your_tavily_api_key
```

---

## Run the Project

```bash
python main.py
```

---

## Workflow

1. User submits a research query.
2. Research Agent searches the web using Tavily.
3. Relevant URLs are collected.
4. BeautifulSoup extracts useful content.
5. Summarization Agent analyzes the information.
6. A concise research report is generated.

---

## Future Enhancements

- Multi-document comparison
- PDF report generation
- Source citation support
- Memory-enabled agents
- Multi-modal document analysis
- Streamlit Web Interface
- Agent orchestration with LangGraph

---

## Applications

- Academic Research
- Market Research
- Competitive Analysis
- Technology Trend Analysis
- Literature Review
- News Summarization
- Business Intelligence

---

## Author

**Anu Shravya**

B.Tech in Computer Science and Engineering (Data Science)

Aspiring Data Scientist | AI & Machine Learning Enthusiast

---

## License

This project is licensed under the MIT License.
