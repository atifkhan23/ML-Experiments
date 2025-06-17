# Project: mlp_classifier_fraud_detection
Description: Add project description here.
# 💳 Credit Card Fraud Detection

## 📌 Objective

The goal of this project is to build a machine learning pipeline that detects fraudulent credit card transactions using standard classification techniques. The model aims to classify transactions into **fraudulent (1)** or **legitimate (0)**.

---

## 🧾 Dataset Information

- The dataset contains anonymized features (V1, V2, ..., V28), along with:
  - `Time`: Seconds elapsed between each transaction and the first transaction
  - `Amount`: Transaction amount
  - `Class`: Target label (1 = Fraud, 0 = Legitimate)

> ⚠️ Due to the highly imbalanced nature of the dataset, proper evaluation metrics are necessary (e.g., confusion matrix, precision-recall).

---

## 🔍 Workflow

### 1. Data Loading
- Load `creditcard.csv` using pandas.

### 2. Preprocessing
- Separate features (`X`) and target (`y`)
- Split the data into train and test sets using `train_test_split`
- Standardize features using `StandardScaler`

### 3. Modeling
- A baseline model is created (e.g., Logistic Regression or other classifiers)
- Performance is evaluated using:
  - Accuracy
  - Confusion Matrix
  - Precision/Recall (optional for future improvement)

### 4. Visualization
- Plot basic graphs to understand performance.

---

## 💡 What You'll Learn

- Handling imbalanced datasets
- Feature scaling and its importance
- Splitting data correctly
- Evaluation of classification models beyond accuracy

---

## 📁 Files

- `fraud_detection.ipynb` — Notebook with code and explanations
- `creditcard.csv` — Dataset (must be placed in your working directory)
- `requirements.txt` — List of dependencies

---

## 🛠️ Setup Instructions

To install the necessary dependencies:

```bash
pip install -r requirements.txt
