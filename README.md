# Nomad: The AI Travel Concierge 🌍✈️

Nomad is a Multi-Agent System (MAS) designed to automate the travel planning process. It features a "Manager-Worker" architecture where specialized agents conduct real-time web research and synthesize data into structured itineraries.

**Track:** Concierge Agents  
**Created for:** Google AI Agents Intensive Capstone 2025

## 🚀 Features
- **Multi-Agent Architecture:** Separates concerns between "Research" (Scout) and "Planning" (Atlas).
- **Tool Use:** Integrated `DuckDuckGo` search for real-time, non-hallucinated data (Weather, Events).
- **Context Awareness:** Passes structured context between agents to maintain logical flow.
- **Gemini Powered:** Uses Google's `gemini-1.5-flash` for high-speed inference.

## 📂 Project Structure
```text
Nomad_Capstone/
├── agents/             # Logic for AI Agents
│   ├── base.py         # Parent class interacting with Gemini API
│   ├── researcher.py   # Agent with Web Search capabilities
│   └── planner.py      # Agent for formatting and itinerary creation
├── tools/              # External Tools
│   └── search_tool.py  # DuckDuckGo search implementation
├── main.py             # CLI Entry point & Orchestrator
├── requirements.txt    # Python dependencies
└── .env                # API Keys (Not included in repo)



**Tech Stack**

Language: Python 3.10+
LLM: Google Gemini 1.5 Flash
Search: DuckDuckGo
Environment: Dotenv