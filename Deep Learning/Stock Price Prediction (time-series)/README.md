# 📈 Stock Price Prediction using RNN/LSTM/GRU

## 📌 Project Overview
This project is about **predicting future stock prices** using deep learning models like **RNN, LSTM, and GRU**.  
We use past stock prices (historical data) to forecast the next day’s price.  

It is a **time series problem**, meaning the order of data matters.  
Unlike traditional ML where rows are independent, here **today’s price depends on previous days**.

---

## 🏦 What is Stock Price?
A **stock** represents a small piece (share) of a company.  

- Example: If you buy a stock of a company, you own a small part of it.  
- Each day, the **price of stock changes** depending on demand, supply, news, and company performance.  

In our dataset:
- Each column (`Stock_1`, `Stock_2`, `Stock_3` …) = price of different companies’ stocks.  
- Each row = a specific date.  

---

## 🔄 How Sequence Works (Time Series)
To predict tomorrow’s stock price, we use the prices from **previous days**.  

👉 Example with a toy dataset (1 stock only):

| Day | Price |
|-----|-------|
| 1   | 100   |
| 2   | 102   |
| 3   | 101   |
| 4   | ???   |

If we choose `time_steps = 3`:
- Input (X) = `[100, 102, 101]`  
- Output (y) = `Day 4 Price`  

This is how **RNN/LSTM/GRU** learn patterns from past values to predict the future.

---

## 🛠 Features of This Project
- Uses **RNN, LSTM, and GRU** for stock price prediction  
- Works on **single stock (univariate)** or **multiple stocks (multivariate)**  
- Uses **MinMax scaling** to normalize values before training  
- Includes evaluation metrics like **RMSE, MAE, and MAPE**  

---

## 📂 Dataset
- Input: CSV file with `Date` + multiple stock columns (e.g., Stock_1 … Stock_5)  
- Example:

Date | Stock_1 | Stock_2 | Stock_3
01-01-2020 | 101.7 | 100.1 | 99.4
02-01-2020 | 102.1 | 99.9 | 98.6


---

## ⚙️ Workflow
1. **Load dataset** (CSV with stock prices)  
2. **Preprocess**: scaling values, handling missing data  
3. **Create sequences**: convert past `time_steps` into input-output pairs  
4. **Build model**: RNN / LSTM / GRU  
5. **Train model** on training data  
6. **Predict** future stock prices  
7. **Evaluate** using RMSE, MAE, MAPE  
8. **Visualize** actual vs predicted stock prices  

---

## 📊 Evaluation Metrics
- **MAE (Mean Absolute Error)** → average error size  
- **MSE (Mean Squared Error)** → penalizes large errors more  
- **RMSE (Root Mean Squared Error)** → most popular for time series  
- **MAPE (Mean Absolute Percentage Error)** → error in percentage  

👉 Lower values = better performance ✅



## 🖼 Visualization
We compare **actual stock price vs predicted stock price** on a time series plot:

Blue Line → Actual Prices
Red Line → Predicted Prices


