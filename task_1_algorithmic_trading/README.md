# 💹 Task 1 — Algorithmic Trading Adventure  

---

## 📘 Project Overview
* Implements a __Golden Cross__ trading strategy using real stock data from Yahoo Finance.
* Developed with a modular, __class-based approach__ in Python.
* Includes data acquisition, cleaning, strategy logic, trade execution, visualization, and performance evaluation.
* Successfully identifies buy/sell signals, calculates profits, and plots equity curves.

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
**(Optional): You can run it in Google Colab or Jupyter simply by only runinng the file *task_1_gcsc.py***

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
<img width="600" height="300" alt="image" src="https://github.com/user-attachments/assets/846d9977-46b2-4b33-a0ac-e135e67937d8" />


---

## 🧑‍💻 Author
**Md. Abu Sufian**  — hisamsufian@gmail.com  

