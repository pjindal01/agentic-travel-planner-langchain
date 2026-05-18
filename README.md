# agentic-travel-planner-langchain
Autonomous AI travel planning agent using LangChain + Groq LLM. Integrates 5 tools (weather, flights, hotels, attractions, budget) with Pydantic-validated inputs. Agent sequences API calls autonomously. Python · LangChain · Groq
# ✈️ Agentic AI Travel Planning Assistant — LangChain + Groq LLM

> An autonomous AI agent that plans complete trips by chaining 5 real-world tools (weather, flights, hotels, attractions, budget). Built with LangChain, Groq LLM, and Pydantic.

---

## 📌 Problem Statement
Planning a trip involves juggling multiple data sources: weather forecasts, flight prices, hotel availability, local attractions, and budget constraints. This project builds an **agentic AI system** that does all of this autonomously — the user states a destination and dates, and the agent sequences tool calls to produce a complete travel plan.

## 🤖 What Makes This "Agentic"?
Unlike a simple chatbot, this system:
- **Decides** which tools to call and in what order
- **Validates** inputs using Pydantic schemas before each API call
- **Chains** outputs from one tool as inputs to the next
- **Reasons** about budget constraints across all bookings

## 🛠️ Tech Stack
`Python` · `LangChain` · `Groq LLM` · `Pydantic` · `Streamlit` · `Pandas`

## 🔧 Tools in the Agent
| Tool | Purpose |
|---|---|
| Weather Tool | Fetches destination weather for travel dates |
| Flights Tool | Searches available flights and prices |
| Hotels Tool | Finds accommodation options |
| Attractions Tool | Recommends local activities |
| Budget Tool | Validates total spend against user budget |

## 📁 Project Structure
```
Agentic_Travel_Planner/
│
├── Agentic_AI_Travel_Planning.ipynb   ← Main notebook
├── requirements.txt
└── README.md
```

## ▶️ How to Run
```bash
# 1. Install dependencies
pip install -r requirements.txt

# 2. Set your Groq API key
# Get a free key at: https://console.groq.com
export GROQ_API_KEY="your_key_here"

# 3. Open and run the notebook
jupyter notebook Agentic_AI_Travel_Planning.ipynb
```

## 🔍 Key Concepts Demonstrated
- **Agentic AI:** agent autonomously decides tool call sequence
- **Tool use with Pydantic validation:** structured, safe API inputs
- **LangChain orchestration:** agent loop with memory and reasoning
- **Groq LLM:** fast inference for real-time agent responses

---
*Project completed as part of AI/ML Internship at Labmentix Pvt. Ltd. (2025–2026)*
