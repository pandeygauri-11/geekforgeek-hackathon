# geekforgeek-hackathon
# Conversational AI for Instant Business Intelligence Dashboards

## 📌 Project Overview
This project builds an intelligent system that allows users to generate business intelligence dashboards using natural language queries.  
Instead of writing SQL or using complex BI tools, users can simply ask questions and get instant data visualizations.

The system uses Conversational AI to understand user queries and generate insights from the database in real time.

---

## 🚀 Features
- Natural Language Query Support
- AI-powered Data Analysis
- Automatic Dashboard Generation
- Interactive Data Visualizations
- Real-time Data Insights

---

## 🛠️ Tech Stack

### Backend
- Python
- FastAPI
- Pandas
- Plotly
- Google Generative AI (Gemini API)
- python-dotenv

### Database
- SQLite

### Frontend
- Streamlit
- HTML
- CSS
- JavaScript
----
**project-folder**
│
├── backend/
│ ├── main.py
│ ├── api.py
│
├── database/
│ └── database.db
│
├── frontend/
│ └── app.py
│
├── .env
├── requirements.txt
└── README.md
---

## ⚙️ Installation

1. Clone the repository

```bash
git clone https://github.com/your-username/your-repo-name.git
---

✅ **Tip for GitHub:**  
After creating the file:

1. Right click in project folder  
2. Create file **README.md**  
3. Paste this content  
4. Commit & push to GitHub

---

1. SYSTEM ARCHITECTURE

                USER
                  |
                  v
        ----------------------
        |   Streamlit UI     |
        |   (Frontend)       |
        ----------------------
                  |
                  | HTTP Request
                  v
        ----------------------
        |   FastAPI Server   |
        |   backend/main.py  |
        ----------------------
                  |
                  v
        -----------------------------
        | Dashboard Controller      |
        | api/dashboard.py          |
        -----------------------------
                  |
                  v
        -----------------------------
        | Dashboard Planner         |
        | dashboard_planner.py      |
        -----------------------------
                  |
                  v
        -----------------------------
        | SQL Generation Engine     |
        | sql_generator.py          |
        -----------------------------
           |                     |
           v                     v

  -----------------------------------------
  | Schema Reader | |     | Intent Engine |
  schema_reader |         | intent_engine |
  ---------------------- ------------------
  | v                    

  -----------------------------------------

  | Context Retrieval (RAG) |
  -----------------------------
  |
  v

| SQL Sanitizer | | SQL Validator | ————————— | v ————————— | SQLite
Database | | marketing.db | ————————— | v ————————— | Chart Selector | |
chart_selector.py | ————————— | v ————————— | Dashboard Builder | |
dashboard_builder.py | ————————— | v JSON RESPONSE | v ————————— |
Streamlit Chart Render | | Plotly Visualization | —————————

2. BACKEND ARCHITECTURE

backend/ │ ├── api │ └── dashboard.py │ ├── database │ ├── db.py │ └──
schema_reader.py │ ├── services │ ├── dashboard_planner.py │ ├──
sql_generator.py │ ├── chart_selector.py │ ├── sql_validator.py │ ├──
sql_sanitizer.py │ ├── sql_corrector.py │ └── dashboard_builder.py │ ├──
ai │ ├── intent_engine.py │ ├── context_retriever.py │ ├──
data_profiler.py │ └── embedding_builder.py │ └── utils └── config.py

3. FRONTEND ARCHITECTURE

frontend/ │ ├── app.py │ ├── components │ ├── chart_renderer.py │ └──
dashboard_layout.py │ ├── services │ └── api_client.py │ ├── config │
└── settings.py │ └── utils └── helpers.py
------














----
