# Assignment 1 — AI Research Agent using CrewAI & LangChain

This project showcases an intelligent **multi-agent research assistant** built using [CrewAI](https://docs.crewai.com/) and [LangChain](https://www.langchain.com/). The system coordinates multiple agents to perform tasks such as web research, summarization, and insight generation — mimicking the collaborative workflow of a human research team.

---

## 🧠 Objective

To build an AI-powered assistant capable of:
- Searching the web for information
- Summarizing relevant results
- Delivering structured answers or reports

---

## 🔧 Tools & Libraries

| Tool | Purpose |
|------|---------|
| 🧩 `CrewAI` | Multi-agent orchestration |
| 🔗 `LangChain` | LLM integration |
| 🔍 `SerperDevTool` | Google Search wrapper |
| 🤖 `Ollama` | Local/hosted language model for inference |

---

## 📂 Project Files

- `AI_Research_Agent.ipynb` — Main notebook demonstrating agent orchestration
- `README.md` — This documentation

---

## 👥 Agents Defined

| Agent Role | Description |
|------------|-------------|
| **Researcher** | Uses SerperDevTool to gather relevant web content |
| **Summarizer** | Condenses the findings into digestible formats |
| **Analyst** | Draws insights or recommendations from the research |

---

## 🚀 How It Works

1. Each agent is created using the `Agent` class.
2. Tasks are assigned using the `Task` class with tools like `SerperDevTool`.
3. The `Crew` executes tasks in a structured workflow (`sequential` or `hierarchical`).
4. The output is a collaboratively constructed research summary.

---

## 🖥️ Ollama Setup Instructions

This project uses [Ollama](https://ollama.com) to run LLMs locally.

### 🪄 Install Ollama

Download and install Ollama:  
🔗 https://ollama.com/download

### 🧠 Run a Model

Open a terminal and run:

'''bash

ollama run mistral

---

### 📊 Output Sample

_You can include screenshots here or sample JSON/text outputs of the agent dialogue or final report._

---

## 🪄 Ideas for Expansion

- Add a memory module to preserve context across queries
- Integrate PDF/doc reader to analyze papers
- Add a frontend UI for natural language prompts

---

## 📌 Status

✅ Agents successfully initialized  
✅ Tasks executed collaboratively  
✅ Produces working research summaries via LLM


## 📜 License

This project is for academic use as part of the Deep Learning coursework.
