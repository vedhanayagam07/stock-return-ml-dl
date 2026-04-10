#  Stock Return Prediction using Machine Learning and LSTM

##  Overview
This project focuses on predicting **next-day stock returns** using both **Machine Learning (ML)** and **Deep Learning (LSTM)** models.  

Unlike traditional approaches that predict stock prices, this project uses **return prediction**, which is more realistic and aligned with financial research.

The system uses historical stock data and applies feature engineering, model training, and evaluation to compare performance across models.

---

##  Objectives
- Predict **next-day stock returns**
- Compare **ML models vs LSTM (Deep Learning)**
- Use **real-world financial metrics**
- Analyze limitations of stock market prediction

---

##  Models Used
### Machine Learning
- Linear Regression
- Random Forest
- XGBoost

###  Deep Learning
- LSTM (PyTorch)

---

##  Evaluation Metrics
- **MAE (Mean Absolute Error)**
- **RMSE (Root Mean Squared Error)**
- **Direction Accuracy** (Up/Down prediction)

---

## Dataset
- S&P 500 historical stock dataset  
- File: `all_stocks_5yr.csv`

Dataset Source:  
https://www.kaggle.com/datasets/rohitjain454/all-stocks-5yr

---

## ⚙️ Project Workflow
1. Data Loading
2. Feature Engineering
   - Returns
   - Moving Averages
   - Volatility
   - Volume changes
3. Train-Test Split (Time-based)
4. Model Training (ML + LSTM)
5. Evaluation & Comparison
6. Visualization

---

##  Key Insight
- Predicting **returns is more reliable than predicting prices**
- All models show **~50% direction accuracy**
- This reflects the **efficient and noisy nature of stock markets**

---

##  Results (Example)

| Model | MAE | RMSE | Direction Accuracy |
|------|-----|------|-------------------|
| Linear Regression | ~0.008 | ~0.012 | ~50% |
| Random Forest | ~0.015 | ~0.018 | ~46% |
| XGBoost | ~0.013 | ~0.017 | ~48% |
| LSTM | ~0.009 | ~0.013 | ~50% |

---

## How to Run

### 1. Install dependencies
```bash
pip install -r requirements.txt
