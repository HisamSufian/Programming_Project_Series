# 🤖 Task 2 — Samsung Phone Advisor API  

---

## 📘 Project Overview
This project creates an **AI-powered API** that intelligently answers questions about Samsung smartphones — including specifications, comparisons, and buying suggestions.  
It uses:
- **FastAPI** for serving responses  
- **PostgreSQL** to store the phone dataset  
- **SentenceTransformer** + **GPT-2 pipeline** for semantic similarity and text generation  

---

## ⚙️ Requirements
```bash
pip install -r requirements.txt
```

### requirements.txt
```
fastapi
uvicorn
sqlalchemy
psycopg2
pandas
sentence-transformers==2.7.0
transformers==4.41.0
torch==2.2.2+cpu
```

*(You can remove `+cpu` if you have GPU support.)*

---

## 🧱 Database Setup
1. Make sure PostgreSQL is running.  
2. Create a database named **samsungdb**:  
   ```sql
   CREATE DATABASE samsungdb;
   ```
3. Open `insert_to_postgres.py` — it automatically creates a table `samsung_phones` and inserts phone specs.  
   ```bash
   python insert_to_postgres.py
   ```

---

## ▶️ Run the API
```bash
uvicorn samsung_advisor_api:app --reload
```

Then open your browser at:  
👉 [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)

---

## 💬 Example Queries

| Example Question | Expected Response |
|------------------|------------------|
| `{ "question": "What are the specs of Samsung Galaxy S23 Ultra?" }` | Returns the phone’s display, camera, battery, and memory specs. |
| `{ "question": "Compare Samsung Galaxy S23 Ultra and S22 Ultra" }` | Compares both models and recommends one. |
| `{ "question": "Which Samsung phone has the best battery under $1000?" }` | Returns the model with the highest battery capacity within that range. |

---

## ⚙️ Internal Logic
- **Intent Detection** → detects if the question is about comparison, specs, or recommendation.  
- **Semantic Model Matching** → finds the closest Samsung model using `SentenceTransformer`.  
- **Comparison Engine** → compares two models based on Camera, Battery, and Display.  
- **Recommendation Engine** → suggests best model by context (gaming, photography, etc.).  

---

## 📂 Folder Structure
```
task_2_samsung_advisor_api/
 ├── samsung_advisor_api.py
 ├── insert_to_postgres.py
 ├── test_selenium.py
 ├── requirements.txt
 └── README.md
```

---

## 🧑‍💻 Author
**Md. Abu Sufian** — hisamsufian@gmail.com  
