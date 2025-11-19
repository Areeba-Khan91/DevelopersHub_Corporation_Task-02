# 📈 Developer Hub – Task 02

## **Predicting Future Stock Prices Using Machine Learning**

---

## 📌 **Clear Problem Statement & Goal**

The objective of this task is to develop and compare two machine learning models—**Linear Regression** and **Random Forest Regressor**—to predict the **next day’s closing price** of a selected stock (AAPL) based on its historical data.

This is a **time-series regression problem**, where the goal is to learn patterns from daily stock features (Open, High, Low, Volume) and accurately forecast the next closing price.

---

## 📊 **Dataset Loading & Preprocessing**

### **📥 Data Source:**

Stock data was downloaded using the **Yahoo Finance (yfinance)** library for the period:
**2015-01-01 to 2025-01-01**

### **📑 Dataset Features Used:**

* Open
* High
* Low
* Volume
* Close (used to create the target variable)

### **🛠️ Feature Engineering – Targ
