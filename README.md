# cybervision
Aggregate real-time cybersecurity threat data from public APIs, analyze and cluster it using NLP and ML, and visualize global threat trends with AI-generated insights.


# 🧠 CyberVision – AI-Powered Cyber Threat Intelligence Dashboard

> A full-stack cybersecurity analytics platform that aggregates real-time threat intelligence from multiple public APIs, applies AI/NLP for automated classification and summarization, and visualizes global attack trends through an interactive dashboard.

---

## 🚀 Overview

**CyberVision** collects live cyber-threat data from sources such as **AlienVault OTX**, **Shodan**, and **VirusTotal**, then processes and analyzes it using natural language processing (NLP) models.  
The app provides a centralized dashboard for researchers, analysts, and security enthusiasts to:
- Identify emerging attack patterns,
- View global heatmaps of threat activity,
- Receive AI-generated insights and summaries.

---

## 🧩 Features

✅ **Threat Data Aggregation**
- Fetches live threat feeds (IPs, domains, malware hashes, ports)
- Normalizes and stores data in MongoDB / Elasticsearch

🧠 **AI/NLP Analysis**
- Summarizes threat reports using transformer models  
- Classifies indicators into categories: *malware, phishing, DDoS, ransomware*, etc.  
- Optional LLM module for generating daily “Threat Digest”

🌍 **Visualization Dashboard**
- React + Mapbox global heatmap of threat origins  
- D3.js/Chart.js analytics for categories, severity, and trends  
- Real-time updates with WebSockets

📡 **Alert & Reporting System**
- Custom alert rules (e.g., “Notify if malware threats spike >25%”)  
- Email / Slack integration  
- PDF & CSV export for analysts

🔐 **Authentication & Security**
- JWT-based authentication  
- Role-based access (Admin, Analyst, Viewer)

---

## 🧰 Tech Stack

| Layer | Technologies |
|--------|---------------|
| **Frontend** | React, Tailwind CSS, Mapbox GL, Chart.js |
| **Backend API** | FastAPI (Python 3.11), Pydantic, Uvicorn |
| **AI & NLP** | Hugging Face Transformers, spaCy, scikit-learn |
| **Database** | MongoDB / Elasticsearch |
| **Task Scheduling** | Celery + Redis |
| **Auth & Security** | JWT / OAuth2 |
| **Deployment** | Docker, Docker Compose, AWS EC2 / Render / Netlify |

---

## 🏗️ Architecture

