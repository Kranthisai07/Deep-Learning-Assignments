# Assignment 1 — AI Research Agent using CrewAI & LangChain

This project showcases an intelligent **multi-agent research assistant** built using [CrewAI](https://docs.crewai.com/) and [LangChain](https://www.langchain.com/). The system coordinates multiple agents to perform tasks such as web research, summarization, and insight generation — mimicking the collaborative workflow of a human research team.

---

## 🧠 Objective

To build an AI-powered assistant capable of:
- Searching the web for relevant content
- Summarizing and analyzing results
- Delivering structured research findings

---

## 🔧 Tools & Libraries

| Tool              | Purpose                                               |
|------------------|-------------------------------------------------------|
| 🧩 `CrewAI`       | Multi-agent orchestration                             |
| 🔗 `LangChain`    | LLM and agent integration                             |
| 🔍 `SerperDevTool`| Web search tool to power real-time research           |
| 🤖 `Ollama`       | Local LLM backend (e.g., Mistral, LLaMA)              |

---

## 👥 Agents Defined

| Agent Role | Description |
|------------|-------------|
| **Researcher** | Uses SerperDevTool to gather relevant web content |
| **Summarizer** | Condenses findings into digestible formats |
| **Analyst** | Draws insights or recommendations from the research |

---

## 🚀 How It Works

1. Agents are initialized and assigned tasks via `CrewAI`.
2. Each agent completes their part using a local LLM powered by Ollama.
3. The result is a complete research report generated collaboratively.

---

## 🖥️ Ollama Setup Instructions

This project uses [Ollama](https://ollama.com) to run LLMs locally.

### 🪄 Install Ollama

Download and install Ollama:  
🔗 https://ollama.com/download

### 🧠 Run a Model

Open a terminal and run:

```bash
ollama run mistral
