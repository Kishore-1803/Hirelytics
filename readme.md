# 🚀 Hirelytics  
### AI-Powered SHL Assessment Recommendation Engine

![License](https://img.shields.io/badge/License-MIT-green.svg)
![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)
![FastAPI](https://img.shields.io/badge/FastAPI-Production-ready-success)
![Docker](https://img.shields.io/badge/Docker-Containerized-blue)
![Azure](https://img.shields.io/badge/Deployed%20on-Azure-0078D4)
![LLM](https://img.shields.io/badge/LLM-Gemini%202.5%20Flash-purple)
![VectorDB](https://img.shields.io/badge/VectorDB-pgvector-orange)

---

## 📌 Overview

**Hirelytics** is an **AI-driven recommendation system** that intelligently suggests the most relevant **SHL assessments** based on a given **job description or hiring context**.

By combining **semantic embeddings**, **hybrid similarity scoring**, and **LLM-powered reranking**, Hirelytics delivers **context-aware, high-precision assessment recommendations** in real time—making it ideal for modern talent acquisition workflows.

---

## 🧠 Key Features

- 🔍 **Context-Aware Recommendations**  
- 🧩 **Hybrid Ranking (70% semantic + 30% keyword)**  
- 🧠 **LLM-Based Reranking (Gemini)**  
- ⚡ **FastAPI + Docker + Azure Deployment**  
- 🌐 **Supports JD text and URLs**  
- 🖤 **Minimal Dark-Mode UI**

---

## 🏗️ System Architecture

```

User Query (Text / URL)
↓
Frontend (HTML + JS)
↓
FastAPI Backend
↓
Sentence-BERT Embeddings
↓
Supabase (Postgres + pgvector)
↓
Hybrid Scoring
↓
Gemini Reranking
↓
Final SHL Recommendations

````

---

## 🧩 Technology Stack

| Layer | Technology |
|------|-----------|
| Frontend | HTML, CSS, JavaScript |
| Backend | FastAPI, Uvicorn |
| Embeddings | SentenceTransformer (`all-mpnet-base-v2`) |
| Vector DB | Supabase (pgvector) |
| LLM | Google Gemini 2.5 Flash |
| Deployment | Docker, Azure App Service |

---

## ⚙️ Installation & Setup

### Clone Repository
```bash
git clone https://github.com/<your-username>/hirelytics.git
cd hirelytics
````

### Setup Environment

```bash
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

### Environment Variables

```env
SUPABASE_URL=your_supabase_url
SUPABASE_KEY=your_supabase_key
GEMINI_API_KEY=your_gemini_api_key
```

### Run Locally

```bash
uvicorn main:app --reload
```

---

## 🔌 API Endpoints

### Health Check

`GET /health`

### Recommendation API

`POST /recommend`

---

## 📈 Performance

| Metric         | Value    |
| -------------- | -------- |
| Mean Recall@10 | **0.62** |

---

## 📂 Project Structure

```
hirelytics/
├── app/
├── data/
├── Dockerfile
├── requirements.txt
├── LICENSE
└── README.md
```

---

## 👤 Author

**Kishore B**

---

## 📄 License

This project is licensed under the **MIT License**.
See the [LICENSE](LICENSE) file for details.

---

⭐ Star the repo if you find it useful!
