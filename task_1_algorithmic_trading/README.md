# 💹 Task 1 — Algorithmic Trading Adventure  

---

## 📘 Project Overview
This project simulates a simple **Golden-Cross Trading Strategy** using Python and historical stock data fetched via `yfinance`.  
The algorithm automatically buys when a *Golden Cross* occurs (50-day MA > 200-day MA) and sells when a *Death Cross* occurs.  
It starts with **$5000 capital** and reports the final profit / loss.

---

## ⚙️ Requirements
```bash
pip install -r requirements.txt
```

### requirements.txt
```
yfinance
pandas
numpy
matplotlib
```

---

## ▶️ How to Run
```bash
python task_1_gcse.py
```

---

## 🧠 Algorithm Steps
1. **Initialize Class** with stock symbol and date range → `class_Name("AAPL","2018-01-01","2023-12-31")`  
2. **Download Data** using `yfinance.download()`  
3. **Clean Data** → remove duplicates & forward-fill NaNs  
4. **Calculate Moving Averages** → 50-day and 200-day  
5. **Detect Golden Cross / Death Cross** → Buy or Sell signals  
6. **Execute Trade Logic** within $5000 budget  
7. **Force Sell on Last Day** if still holding  
8. **Print Final Summary** → Profit or Loss  

---

## 💻 Sample Output
```
Trading Results
✅Initial Budget: $5000.00
✅Final Portfolio Value: $11661.68
💰Total Profit/Loss: $6661.68
📈Number of Trades: 10
📈Average Profit/Loss per Trade: $666.17
Profit Percentage: 133.23%
```

---

## 📊 Visualization 
The script plots closing price with 50 / 200 moving averages and trade markers for buy/sell signals.

---

## 🧑‍💻 Author
**Md. Abu Sufian**  — hisamsufian@gmail.com  

