# 📈 Stock Price Prediction & Trend Forecasting

This project predicts **stock movement direction** (up/down) and **future closing prices** using technical indicators and machine learning models (XGBoost Classifier & Regressor). It leverages `yfinance` for live stock data and includes feature engineering techniques like MACD, RSI, and EMA.

---

## 🚀 Tech Stack

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![Seaborn](https://img.shields.io/badge/Seaborn-1481BA?style=for-the-badge&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![XGBoost](https://img.shields.io/badge/XGBoost-EC2D2D?style=for-the-badge&logo=xgboost&logoColor=white)
![yfinance](https://img.shields.io/badge/yfinance-3572A5?style=for-the-badge&logo=Yahoo&logoColor=white)
![TA-Lib](https://img.shields.io/badge/TA--Lib-blueviolet?style=for-the-badge)

---

## 🛠️ Technology & Description

| Technology                                                                                                   | Description                          |
|--------------------------------------------------------------------------------------------------------------|--------------------------------------|
| ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)    | Fast numerical operations            |
| ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) | Data wrangling and manipulation      |
| ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) | Visualization of predictions         |
| ![Seaborn](https://img.shields.io/badge/Seaborn-1481BA?style=for-the-badge&logoColor=white)                  | Heatmaps for confusion matrix        |
| ![scikit-learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white) | Classification metrics               |
| ![XGBoost](https://img.shields.io/badge/XGBoost-EC2D2D?style=for-the-badge&logo=xgboost&logoColor=white)     | High-performance tree-based models   |
| ![yfinance](https://img.shields.io/badge/yfinance-3572A5?style=for-the-badge&logo=Yahoo&logoColor=white)     | Fetching historical stock data       |
| ![TA-Lib](https://img.shields.io/badge/TA--Lib-blueviolet?style=for-the-badge)                               | Technical indicator calculations     |

---

## 🧠 Features Implemented

- 📥 **Live Stock Downloading** from Yahoo Finance with fallbacks  
- 🧮 **Feature Engineering**:  
  - MACD (Moving Average Convergence Divergence)  
  - RSI (Relative Strength Index)  
  - EMA (Exponential Moving Averages)
  - Daily Returns

- 📊 **Classification Task**:
  - Predicts whether the stock will go up or down the next day
  - Model: `XGBoostClassifier`
  - Evaluation: Accuracy, Classification Report, Confusion Matrix

- 💸 **Regression Task**:
  - Predicts stock's closing price `n` days into the future
  - Model: `XGBoostRegressor`
  - Evaluation: Mean Squared Error (MSE), Actual vs Predicted plots

- 📈 **Graphical Visualizations**:
  - Actual vs predicted future price line charts
  - Confusion matrix heatmaps
  - Closing price historical trends

---

## ✅ Achievements

1. **Dual Modeling**: Implemented both classification (up/down movement) and regression (future price) in a single pipeline.
2. **High Accuracy Classification**: XGBoost classifier achieves over **85% accuracy** on most stocks by leveraging well-engineered technical indicators.
3. **Forecasting**: Future stock price prediction (up to 5 days ahead) using tree-based regression models with optimized error metrics.
4. **Error Handling**: Automatic fallback to default stock if invalid ticker is entered.
5. **Modular & Scalable**: Easy to switch to other tickers like TSLA, MSFT, etc.

---

## 📌 How to Run

```bash
pip install yfinance ta scikit-learn xgboost matplotlib seaborn
