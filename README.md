# 🧠 AI-Powered Multilingual Airport Assistance Chatbot — Phase 1 (Prototype)

### 🎓 Final Year Project – DHA Suffa University  
**Supervisor:** Sir Ayub Kamal  
**External Co-Supervisor:** Sir Shahab  
**Team Lead:** Muhammad Rayyan Ayub  
**Team Members:** 
**Duration:** Phase 1 (Week 1–10)  

---

## 🚀 Project Overview

This project aims to develop an **AI-powered multilingual chatbot** designed to assist **airport passengers** by providing real-time information in **English, Urdu, and Roman Urdu**.  
The system will handle queries related to **flight details**, **check-in**, **baggage**, **lost and found**, and **terminal guidance** — with **context-aware interactions** for both **Departure** and **Arrival** terminals.

The chatbot will use **LoRA fine-tuning** applied to **Google’s Multilingual BERT (mBERT)** and **Meta’s XLM-BERT** models to enhance understanding of Urdu and Roman Urdu queries.  
This repository documents **Phase 1 (Prototype Stage)**, focusing on dataset creation, environment setup, and backend preparation.

---

## 🎯 Objectives of Sub Phase 1
1. Set up a well-structured GitHub repository for the project.  
2. Define dataset schema and intents for airport-related interactions.  
3. Collect and prepare **synthetic multilingual data** (English, Urdu, Roman Urdu).  
4. Establish development environment and folder structure.  
5. Prepare documentation and project charter for supervisor review.  

---

## 📁 Repository Structure

airport-chatbot-prototype/
├─ data/
│ ├─ raw/ # Unprocessed synthetic data
│ ├─ processed/ # Cleaned & structured data (CSV/JSON)
│ └─ README.md
│
├─ backend/
│ └─ app/ # FastAPI backend and endpoints ( Sub Phase 3+)
│
├─ frontend/
│ └─ static/ # Chat UI files (HTML, JS) for prototype
│
├─ models/ # Fine-tuned LoRA models and configurations
│
├─ docs/
│ ├─ PROJECT_CHARTER.md # Project purpose, scope, and objectives
│ ├─ DATA_SCHEMA.md # Dataset structure and labeling details
│ ├─ CONTRIBUTING.md # Branching and workflow rules
│ └─ MEETING_LOGS.md # Weekly updates and notes
│
├─ experiments/ # Model training or notebook tests
│
├─ .github/
│ ├─ ISSUE_TEMPLATE.md
│ ├─ PULL_REQUEST_TEMPLATE.md
│ └─ workflows/ # Optional CI/CD actions
│
├─ .gitignore
├─ requirements.txt # Python dependencies
└─ README.md # This file

yaml
Copy code

---

## 🧠 Core Features (Planned)

| Feature | Description |
|----------|-------------|
| **Multilingual Support** | Understands English, Urdu (script), and Roman Urdu |
| **Terminal Awareness** | Distinguishes queries from Departure vs Arrival |
| **LoRA Fine-Tuning** | Efficient adaptation of mBERT & XLM-BERT for Urdu/Roman Urdu |
| **FastAPI Backend** | REST API for handling user queries |
| **Synthetic Dataset** | Realistic passenger queries generated for training |
| **Extensible Design** | Modular architecture for easy scaling & deployment |

---

## 🧩 Sub Phase 1 Deliverables

| Deliverable | Description |
|--------------|-------------|
| ✅ Dataset v1 | Synthetic multilingual dataset (300–500 queries) |
| ✅ Documentation | Project Charter + Dataset Schema |
| ✅ Environment Setup | Python, FastAPI, Transformers, and repo structure |
| ✅ Version Control | Branching rules and PR workflow implemented |

---

## ⚙️ Technology Stack

| Category | Tools / Frameworks |
|-----------|-------------------|
| **Programming Language** | Python 3.10+ |
| **Backend Framework** | FastAPI |
| **NLP Models** | mBERT, XLM-BERT (fine-tuned via LoRA) |
| **Data Handling** | Pandas, Datasets, Scikit-learn |
| **Version Control** | Git, GitHub |
| **Collaboration** | Google Drive, Notion, Discord/WhatsApp |
| **Environment** | Jupyter Notebook, Google Colab (GPU support) |

---

## 🧱 Branching Workflow

| Branch | Purpose |
|---------|----------|
| **main** | Stable branch, managed by Team Lead (Rayyan) |
| **dev** | Integration branch for reviewed updates |
| **feature/** | Feature-specific branches (e.g., `feature/data-collection`) |

🔒 **Note:** Team members must not push directly to `main`.  


---

## 🧩 How to Get Started

### 1. Clone the Repository
```bash
git clone https://github.com/<username>/airport-chatbot-prototype.git
cd airport-chatbot-prototype
2. Create Virtual Environment & Install Dependencies
bash
Copy code
python -m venv venv
source venv/bin/activate     # (Linux/Mac)
venv\Scripts\activate        # (Windows)
pip install -r requirements.txt
3. Verify Setup
bash
Copy code
python --version
pip list
🧠 Example Data Schema (for Phase 1 Dataset)
Query	Language	Intent	Terminal	Response
Where is my gate?	English	Directions	Departure	Your gate number is displayed on the flight board.
میرا گیٹ کہاں ہے؟	Urdu	Directions	Departure	آپ کا گیٹ نمبر فلائٹ بورڈ پر درج ہے۔
Mera flight kab niklay ga?	Roman Urdu	Flight Info	Departure	Aapka flight shaam 7:30 baje niklay ga.

🗓️ Weekly Progress Tracking (Phase 1)
Week	Focus Area	Deliverable
Week 1	Environment & Repo Setup	Folder structure + Dataset schema
Week 2	Data Creation & Validation	Multilingual dataset + Documentation

📜 License
This project is developed as part of the Final Year Project at DHA Suffa University and is not open for public distribution without supervisor permission.



“Empowering smarter travel through multilingual AI — one conversation at a time.”
