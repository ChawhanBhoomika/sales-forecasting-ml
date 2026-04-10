# 📈 Sales Forecasting using Time Series + Machine Learning

## 🔹 Project Overview
This project focuses on forecasting retail sales using historical data by combining time series analysis and machine learning techniques. The goal is to build a robust model that can predict future sales and help in better inventory and demand planning.

---

## 🔹 Problem Statement
Accurate sales forecasting is critical for retail businesses to:
- Avoid stockouts
- Reduce overstocking
- Optimize supply chain operations

This project predicts **future daily sales at store level** using historical data.

---

## 🔹 Dataset
- Source: Kaggle (Rossmann Store Sales)
- Records: ~1 million rows
- Features:
  - Date, Store, Sales (target)
  - Customers, Promotions
  - Holidays, Store details

---

## 🔹 Tech Stack
- **Python**
- **Pandas, NumPy** → Data processing  
- **Matplotlib, Seaborn** → Visualization  
- **Scikit-learn** → ML models  
- **XGBoost** → Advanced modeling  

---

## 🔹 Project Workflow

### 1. Data Preprocessing
- Merged multiple datasets
- Handled missing values
- Converted date column to datetime
- Removed closed stores and zero sales

### 2. Exploratory Data Analysis (EDA)
- Identified trends and seasonality
- Analyzed promotion impact
- Observed strong correlation between customers and sales

### 3. Feature Engineering
- Extracted time-based features (year, month, weekday)
- Created **lag features** (Lag_1, Lag_7, Lag_30)
- Added **rolling mean features**
- Encoded categorical variables

### 4. Model Building
- Baseline model (lag-based)
- Random Forest
- XGBoost (final model)

### 5. Model Evaluation
- Metrics used:
  - MAE (Mean Absolute Error)
  - RMSE (Root Mean Squared Error)
- Compared all models against baseline

### 6. Hyperparameter Tuning
- Used **RandomizedSearchCV**
- Improved model performance and generalization

---

## 🔹 Results
- XGBoost outperformed baseline and Random Forest
- Lag features were the most important predictors
- Promotions significantly increased sales

---

## 🔹 Key Insights
- Sales show strong **seasonality (weekly & monthly)**
- Promotions have a **major impact on demand**
- Past sales strongly influence future sales
- Customer count is highly correlated with sales

---

## 🔹 Project Structure
