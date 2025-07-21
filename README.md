# 🤖 QA-Agent

**QA-Agent** is an intelligent question-answering system built using **FastAPI**, **LangChain**, and **OpenAI's LLMs**. It is capable of:

- Searching the web for context
- Summarizing relevant information
- Answering user queries with traceable and explainable outputs

This project is ideal for building automated agents capable of giving well-informed answers using up-to-date web data.

## 🚀 Features

- 🔍 Web Search Integration (e.g., DuckDuckGo)
- 🧠 Summarization via LangChain Chains
- 🤖 LLM-powered QA (OpenAI)
- ⚡ FastAPI backend with auto-generated Swagger UI (`/docs`)
- 🐳 Docker support for easy deployment

## 🛠️ Technologies Used

- **FastAPI** – backend framework
- **LangChain** – for chaining prompts and tools
- **OpenAI API** – LLM for answering questions
- **DuckDuckGo Search API** – for external web search
- **Playwright / Requests / BeautifulSoup** – for scraping and HTML cleaning
- **Docker** – for containerization

## 🧾 Project Structure

```text
QA-Agent/
├── .env.example
├── .gitignore
├── Dockerfile
├── Makefile
├── docker-compose.yaml
├── main.py
├── qa_agent.py
├── requirements.txt
├── scraping_tool.py
├── search_tool.py
├── sites_data.csv
└── README.md
```

## 📥 Installation & Setup

### 🔁 Clone the Repository

```bash
git clone https://github.com/Imaad00/QA-Agent.git
cd QA-Agent

# Create virtual environment
python -m venv venv

# Activate it:
# On Windows
venv\Scripts\activate

# On macOS/Linux
source venv/bin/activate

# 📦 Install Dependencies
pip install -r requirements.txt

# ▶️ Run the FastAPI Server
python main.py

# Server will start
localhost:8000/docs
```
## 🔑 Set Up Environment Variables

Copy the example `.env` file:

```bash
cp .env.example .env
```
Then open `.env` and add your Google API key and Tavily API key:

```ini
GOOGLE_API_KEY=your_google_api_key_here
TAVILY_API_KEY=your_tavily_api_key_here


