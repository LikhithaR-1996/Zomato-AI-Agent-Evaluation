# 🍽️ Zomato Bangalore Restaurant Intelligence & AI Agent Evaluation

A Data Analytics and AI Agent Evaluation project built using the Zomato Bangalore dataset.

This project combines traditional data analysis with modern AI agent evaluation techniques. It starts by identifying key factors influencing restaurant success in Bangalore and extends those insights into an AI-powered business advisor capable of answering restaurant strategy questions using natural language.

---

## 📌 Project Overview

The objective of this project was to understand what drives restaurant success on Zomato Bangalore and then build an AI agent that can answer business questions based on those insights.

The project is divided into two parts:

### Part 1 — Restaurant Analytics
Performed exploratory data analysis on 41,263 restaurants to identify patterns related to:

- Location performance
- Cuisine popularity
- Price range impact
- Online ordering influence
- Table booking influence

### Part 2 — AI Agent Evaluation
Built an AI-powered restaurant advisor using:

- Router
- Skills
- Memory
- State Management

The agent answers business questions and is evaluated using LLM-as-a-Judge techniques for quality, faithfulness, and relevance.

---

## 🎯 Business Questions Answered

The AI Agent answers questions such as:

1. Which location should I open my restaurant in Bangalore?
2. What cuisine type gets the highest ratings?
3. What price range should I target?
4. Should I offer table booking?
5. Does online ordering significantly improve ratings?

---

## 🛠️ AI Agent Architecture

The agent consists of four core components:

### Router
Routes user questions to the appropriate skill.

### Skills
Specialized handlers for:

- Location Analysis
- Cuisine Analysis
- Pricing Analysis
- Service Analysis

### Memory
Stores verified insights extracted from the Zomato dataset.

### State Management
Tracks agent execution stages:

```text
RECEIVING
→ ROUTING
→ PROCESSING
→ COMPLETE
```

---

## 📊 Agent Evaluation Framework

Implemented an LLM-as-a-Judge evaluation system inspired by concepts learned from DeepLearning.AI's Agent Evaluation course.

### Evaluation Metrics

- Faithfulness Score
- Relevance Score
- Hallucination Detection
- Overall Score
- Pass / Fail Status

### Quality Gate

An answer passes only if:

- Faithfulness ≥ 0.7
- Relevance ≥ 0.7
- Hallucination = NO

---

## 🔍 Tracing & Observability

Implemented custom tracing concepts inspired by OpenTelemetry.

### Trace

A complete run of the AI agent from question to final evaluation.

### Spans

Individual steps inside a trace:

- Routing Span
- Skill Execution Span
- Judge Evaluation Span

Tracked metrics include:

- Total Execution Time
- Skill Execution Duration
- Evaluation Duration

---

## 📈 Power BI Dashboard

Developed interactive dashboards to monitor:

### Restaurant Analytics

- Top Locations by Rating
- Top Cuisines by Rating
- Rating by Price Range
- Online Ordering Impact
- Table Booking Impact

### AI Agent Evaluation

- Average Faithfulness Score
- Average Relevance Score
- Pass Rate
- Hallucination Count
- Agent Quality Status
- Response Time Metrics

---

## 🔑 Key Business Insights

| Factor | Finding |
|----------|----------|
| Location | Lavelle Road and Koramangala showed the highest average ratings |
| Cuisine | Malaysian, Modern Indian, and Japanese cuisines performed strongly |
| Price Range | Premium restaurants generally achieved higher ratings |
| Online Ordering | Minimal rating impact |
| Table Booking | Strongest positive impact on ratings |

---

## 🧰 Technologies Used

### Data Analytics

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn

### AI Agent Evaluation

- Groq API
- Llama 3.3 70B
- Prompt Engineering
- LLM-as-a-Judge
- Agent Evaluation Frameworks

### Visualization

- Power BI

### Development Environment

- Jupyter Notebook

---

## 📂 Project Structure

```text
Zomato-AI-Agent-Evaluation
│
├── notebooks
│   ├── Zomato_Bangalore_Analysis.ipynb
│   └── Zomato_AI_Agent_Evaluation.ipynb
│
├── data
│   ├── zomato_agent_evaluation_full.csv
│   └── zomato_agent_summary.csv
│
├── dashboard
│   └── Zomato_Agent_Dashboard.pbix
│
├── screenshots
│   ├── dashboard_overview.png
│   └── evaluation_dashboard.png
│
├── requirements.txt
├── .gitignore
└── README.md
```

---

## 📚 Learning Outcomes

Through this project I gained hands-on experience with:

- Exploratory Data Analysis
- Business Intelligence
- AI Agent Architecture
- Agent Routing
- Memory & State Management
- LLM Evaluation
- Hallucination Detection
- Tracing & Observability Concepts
- Power BI Dashboard Development

---

## 📊 Dataset

Dataset: Zomato Bangalore Restaurants

- Raw Dataset: 51,717 records
- Cleaned Dataset: 41,263 records

Source: Kaggle Zomato Bangalore Restaurants Dataset

---

## 🚀 Future Improvements

- OpenTelemetry Integration
- Arize Phoenix Integration
- Larger Evaluation Dataset
- Retrieval-Augmented Generation (RAG)
- Human Evaluation Pipeline
- Multi-Agent Architecture

---

## 👤 Author

Likhitha R

Aspiring Data & AI Professional interested in Data Analytics, AI Agents, Document Intelligence, Business Intelligence, and AI Evaluation.
