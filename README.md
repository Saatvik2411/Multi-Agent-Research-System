# Multi-Agent Research Explorer

A university showcase project built with Python, Streamlit, and LangChain to demonstrate an intelligent multi-agent search and reasoning system.

## What this project does

This app uses multiple chained agents to:
- search the web and documents for relevant information,
- reason over the input query,
- and return concise answers with real-time retrieval support.

It is designed as a lightweight research assistant that combines:
- a Streamlit front-end for interactive use,
- LangChain agent orchestration,
- OpenAI as the language model backend,
- and external tools such as web search and parsing.

## Why it is unique

- **Multi-agent workflow**: not a simple chat app, but a pipeline of agents with specialized roles.
- **Modular design**: `agents.py`, `pipeline.py`, and `tools.py` separate concerns cleanly.
- **Production-ready patterns**: uses `.env` for credentials and `.gitignore` to keep secrets out of version control.
- **University-ready demo**: easy to explain, extend, and present.

## Project structure

- `app.py` — Streamlit application entry point.
- `agents.py` — builds and configures the LangChain agents.
- `pipeline.py` — orchestrates the multi-agent workflow.
- `tools.py` — supports external tool integrations and helpers.
- `requirements.txt` — lists Python dependencies.
- `.env` — holds private API keys (not checked into Git).
- `.gitignore` — excludes `.venv`, `.env`, and Python caches.

## Setup instructions

1. Clone the repo.
2. Create and activate a virtual environment:
   ```bash
   python -m venv .venv
   .venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Create a `.env` file with your OpenAI key:
   ```text
   OPENAI_API_KEY=your_openai_api_key_here
   ```
5. Run the app:
   ```bash
   streamlit run app.py
   ```

## How to use

- Open the Streamlit URL shown in the terminal.
- Enter a research or search query.
- The multi-agent system will generate a response using retrieval, reasoning, and text generation.

## Dependencies

This project uses:
- `langchain`
- `langchain-core`
- `langchain-community`
- `langchain-openai`
- `openai`
- `streamlit`
- `beautifulsoup4`, `requests`, `lxml`
- `python-dotenv`
- `aiohttp`, `pandas`, `tiktoken`, `rich`

