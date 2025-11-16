
# 📈 Stock Volatility Prediction Using Machine Learning

Predicting short-term stock volatility using historical OHLC data, engineered financial features, and machine learning models.

---

## 🚀 Overview

This project focuses on forecasting **next-day volatility** using price-based features and rolling statistical indicators.
The study evaluates two models:

* **Linear Regression** → baseline, interpretable
* **Random Forest Regressor** → captures nonlinear patterns

The goal is to compare performance and understand how well simple ML techniques can model short-term volatility for stocks such as **ADANIPORTS**.

---

## 📊 Problem Statement

Volatility represents **risk** and **uncertainty** in stock price movements.
Accurate volatility forecasting is essential for:

* Risk management
* Intraday strategies
* Option pricing
* Portfolio allocation

This project demonstrates how ML can supplement traditional financial models for practical forecasting.

---

## 🛠️ Methodology

### 1. **Data Preprocessing**

* Used NIFTY50 stock market dataset
* Cleaned missing values (forward fill)
* Sorted chronologically
* Added engineered features

### 2. **Feature Engineering**

Features include:

* Daily returns & log returns
* Rolling mean & rolling standard deviation (5/10/30-day windows)
* Lagged returns
* Technical indicators (RSI, Bollinger Bands, ATR)
* Squared & absolute returns

These features capture both **trend** and **volatility clustering** effects.

---

## 📘 Models Used

### 🔹 **Linear Regression (Baseline)**

* Interpretable
* Works well for simple linear relationships
* Requires scaling

### 🔹 **Random Forest Regressor**

* Captures nonlinearity & feature interactions
* Scale-invariant
* More robust during volatility spikes

---

## 🧪 Evaluation Metrics

The models are evaluated using:

* **MAE** (Mean Absolute Error)
* **MSE** (Mean Squared Error)
* **R² Score**

A chronological **80-20 train–test split** ensures no data leakage.

---

## 📈 Results Summary

* Random Forest performs slightly better than Linear Regression
* Both models capture general volatility trends
* Random Forest handles **abrupt market shocks** more effectively
* Large volatility spikes remain challenging

---

## 📁 How to Run the Project

### 1. Clone the repository

```bash
git clone (https://github.com/swarnaliiiiii/simple-volatility-prediction-system.git)
cd volatility-prediction
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the notebook

```bash
jupyter notebook
```

Open:
`notebook/volatility_prediction.ipynb`

---

## 🔮 Future Work

Potential improvements:

* Add macroeconomic indicators (VIX, FII data)
* Integrate sentiment analysis using news + social media
* Try advanced models:

  * XGBoost
  * LSTM / GRU
  * Hybrid statistical + ML models
* Deploy a real-time prediction system with retraining

---

## 👤 Author

**Swarnali**
Engineering student | Machine Learning & AI Projects

---

If you want, I can also:

✅ Generate the repository folder structure
✅ Create `requirements.txt`
✅ Add badges / shields for GitHub
✅ Make a more aesthetic or minimal README
Just tell me!
