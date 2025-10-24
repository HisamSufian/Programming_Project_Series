# 🚀 Python Programming Project — by Sufian

---

## 📁 Overview
Two independent Python projects:

| # | Project | Domain | Description |
|--|--|--|--|
| 1 | Algorithmic Trading Adventure | Finance + Data Science | Golden-Cross trading strategy using yfinance & pandas |
| 2 | Samsung Phone Advisor API | AI + Web + NLP | FastAPI service that answers Samsung-related questions intelligently |

---

### 🛠 Common Requirements
- Python 3.11+
- `pip`
- (PostgreSQL required only for Task 2)

---

### ▶️ Run Each Task

**Task 1:**
```bash
cd task_1_algorithmic_trading
pip install -r requirements.txt
python task_1_gcse.py
```

---

**Task 2:**
```bash
cd task_2_samsung_advisor_api
pip install -r requirements.txt
python insert_to_postgres.py
uvicorn samsung_advisor_api:app --reload
```

---

Then open: http://127.0.0.1:8000/docs

---
📂 Folder Structure
Python_Programming_Task/
 ├── task_1_algorithmic_trading/
 ├── task_2_samsung_advisor_api/
 └── README.md

---

Author: Md. Abu Sufian — hisamsufian@gmail.com
---
