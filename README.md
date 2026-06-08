# Introduction to LangChain v1

A beginner-friendly learning repo for LangChain v1. Each notebook has working code with notes explaining the concept in plain English.

---

## Topics Covered

| # | Topic | Notebook |
|---|-------|----------|
| 1 | Create a simple agent | [1-create-agent.ipynb](langchain/1-create-agent.ipynb) |
| 2 | Chat models (`init_chat_model` vs `ChatGroq`) | [2-chat-model.ipynb](langchain/2-chat-model.ipynb) |
| 3 | Streaming responses | [3-streaming.ipynb](langchain/3-streaming.ipynb) |
| 4 | Batch requests | [4-batch.ipynb](langchain/4-batch.ipynb) |
| 5 | Tools (create, bind, use with agent) | [5-tools.ipynb](langchain/5-tools.ipynb) |
| 6 | Types of messages | [6-messages.ipynb](langchain/6-messages.ipynb) |

---

## Quick Concept Summary

- **Chat Model** — The AI brain. Use `init_chat_model("groq:model-name")` to create one.
- **Agent** — A smart assistant that automatically decides which tools to use. Created with `create_agent(...)`.
- **Tool** — A Python function with `@tool` decorator that the agent can call for real-world data.
- **Streaming** — Get AI response word by word using `.stream()` instead of waiting for the full answer.
- **Batch** — Send multiple prompts at once using `.batch([...])` for efficiency.
- **Messages** — Conversations are lists of `SystemMessage`, `HumanMessage`, `AIMessage`, `ToolMessage`.

---

## Setup

```bash
uv sync

# Add your API key to .env
GROQ_API_KEY=your_key_here
```
