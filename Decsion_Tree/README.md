# Project: Decsion_Tree
Description: Add project description here.
# Data Analysis and Churn Prediction

## 📂 Project Description

This project consists of two main datasets:

1. **California Housing Dataset**  
   Contains housing statistics from California including median income, location, number of rooms, and proximity to the ocean. The goal is to perform data cleaning, EDA, and predictive modeling on housing value.

2. **Customer Churn Dataset**  
   Telecom customer dataset used to identify factors influencing customer churn. Includes demographic data, service usage, contract type, payment methods, and churn reason.

---

## 📌 Tasks Overview

### 1. California Housing Analysis
- Handle missing values (e.g. `total_bedrooms`)
- Visualize geographical and income distribution
- Model housing prices using regression (Linear, XGBoost, CatBoost, etc.)
- Evaluate with metrics like RMSE and R²

### 2. Customer Churn Analysis
- Handle missing categorical values (e.g. `Internet Type`, `Churn Reason`)
- Perform one-hot encoding on categorical columns
- Classify churn status using classification models (Logistic Regression, XGBoost, etc.)
- Evaluate using accuracy, precision, recall, and confusion matrix

---

## ⚙️ Requirements

Install all dependencies using:

```bash
pip install -r requirements.txt
