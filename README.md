# 🧠 TweetGen-Evaluator: LangGraph Tweet Refinement Agent

This project is an **agentic AI system** built using [LangGraph](https://github.com/langchain-ai/langgraph) and [OpenAI], designed to **generate high-quality tweets** based on a given topic. It uses a multi-step refinement loop where each tweet is evaluated and improved until it meets quality standards.

---

## 🚀 Features

- 🔁 **Multi-agent loop**: Generate → Evaluate → Feedback → Refine
- 🧠 **LLM-powered tweet writing** using OpenAI GPT models
- 📊 **Evaluation node** checks quality and gives feedback
- 🎯 Stops when the tweet is either accepted or max iterations are reached
- ⚙️ Built with **LangGraph**, **LangChain**, and **Python**

---

## 🛠️ How It Works

1. **Input** a topic (e.g. "LangChain + LangGraph").
2. The **LLM generates a tweet**.
3. An **evaluator node** reviews the tweet and labels it:
   - ✅ Accepted
   - ❌ Needs Improvement
4. If the tweet is rejected, a **feedback loop** improves it using suggestions.
5. The process repeats until:
   - Tweet is accepted, or
   - Maximum iterations (e.g. 5) are reached

---

## 📂 Project Structure

```bash
.
├── X_post.ipynb         # Jupyter Notebook with full LangGraph logic
├── .env                 # OpenAI API Key (not shared)
└── README.md            # This file
