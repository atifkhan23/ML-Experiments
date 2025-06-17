# Project: logistic_regression_titanic_data_set
Description: Add project description here.
# Credit Card Fraud Detection

## 📌 Objective

This project is focused on detecting fraudulent credit card transactions using machine learning techniques. The dataset is highly imbalanced and contains real-world transactions, making it ideal for classification tasks.

---

## 🧾 Dataset

- **File**: `creditcard.csv`
- **Shape**: 284,807 rows × 31 columns
- **Target**: `Class`
  - `0`: Legitimate
  - `1`: Fraudulent
- Most features are anonymized via PCA transformation (`V1`, `V2`, ..., `V28`) plus `Amount` and `Time`.

---

## 🔍 Workflow

1. Load and explore dataset
2. Preprocess features
   - Drop `Class` column from `X`
   - Apply **StandardScaler**
3. Split data using `train_test_split` (80/20)
4. Train a classifier (e.g., Logistic Regression, Random Forest)
5. Evaluate model using:
   - Accuracy
   - Confusion matrix
   - ROC AUC (optional)

---

## 📁 Files

- `fraud_detection.py` — Main Python script
- `creditcard.csv` — Dataset
- `requirements.txt` — Python dependencies

---

## 🔧 Setup

Install all required packages using:

```bash
pip install -r requirements.txt
