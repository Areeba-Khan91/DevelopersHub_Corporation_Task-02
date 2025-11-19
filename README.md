# 📈 Developer Hub – Task 02

## **Predicting Future Stock Prices Using Machine Learning**

---

## 📌 **Problem Statement & Goal**

The objective of this task is to develop and compare two machine learning models—**Linear Regression** and **Random Forest Regressor**—to predict the **next day’s closing price** of a selected stock (AAPL) based on its historical data.

This is a **time-series regression problem**, where the goal is to learn patterns from daily stock features (Open, High, Low, Volume) and accurately forecast the next closing price.

---

## 📊 **Dataset Loading & Preprocessing**

### **📥 Data Source**

Stock data was downloaded using the **Yahoo Finance (yfinance)** library for the period:  
**2015-01-01 to 2025-01-01**

### **📑 Dataset Features Used**

* Open
* High
* Low
* Volume
* Close (used as the target variable for prediction)

### **🛠️ Feature Engineering**

* **Target Variable:** Next day’s closing price
* **Lag Features:** Previous day’s OHLCV values used to predict the next closing price
* **Train-Test Split:** 80% train, 20% test
* **Scaling:** Features scaled using StandardScaler to improve model performance

---

## 🤖 **Models Applied**

### **1️⃣ Linear Regression (Baseline)**

* Captures simple linear relationships between input features and target
* Provides a baseline for comparison

### **2️⃣ Random Forest Regressor (Advanced)**

* Ensemble tree-based model capturing non-linear relationships
* Can handle complex interactions between features
* Hyperparameters used:
  * `n_estimators=500`
  * `max_depth=None`
  * `random_state=42`

---

## 📏 **Model Evaluation**

Models were evaluated using:

* **MAE (Mean Absolute Error)** – measures average absolute difference between predictions and actual values  
* **RMSE (Root Mean Squared Error)** – penalizes larger errors more heavily  

📌 **Results:**  
* Random Forest Regressor outperformed Linear Regression with lower MAE and RMSE, capturing complex trends in stock price data better.

---

## 📈 **Key Insights**

* Historical OHLCV data can provide valuable signals for predicting short-term stock movements
* Random Forest Regressor is highly effective for capturing non-linear patterns in time-series data
* Proper preprocessing, including feature scaling and lag feature creation, is crucial for accurate predictions

---

## 🧾 **Code Included**

The project includes:

* Data download and loading using `yfinance`
* Feature engineering and target creation
* Preprocessing (scaling, train-test split)
* Model training (Linear Regression + Random Forest)
* Evaluation using MAE & RMSE
* Visualization of actual vs predicted stock prices

---

## ✅ **Conclusion**

This task demonstrates that **Random Forest Regressor is superior for short-term stock price prediction** compared to Linear Regression.  
The notebook provides a strong foundation for further time-series modeling, including advanced methods like LSTM, XGBoost, or ensemble stacking.

---

**Author:** Areeba Khan  
**Internship:** Developer Hub  
**Task:** 02 – Predicting Future Stock Prices Using Machine Learning
