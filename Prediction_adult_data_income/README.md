# Project: Prediction_adult_data_income
Description: Add project description here.
# 👨‍💼 Income Classification with Gaussian Naive Bayes

This project uses the **UCI Adult Income Dataset** to predict whether a person earns **more than $50K/year** based on census information using a custom **Gaussian Naive Bayes classifier**.

---

## 📌 Objectives

- Clean and preprocess the UCI Adult dataset
- Encode categorical variables numerically
- Train a Gaussian Naive Bayes model from scratch
- Evaluate model performance using common classification metrics

---

## 📊 Dataset Details

- **Source:** [UCI Machine Learning Repository - Adult Data Set](https://archive.ics.uci.edu/ml/datasets/adult)
- **Features:**
  - Age, workclass, education, marital-status, occupation, relationship, race, sex, hours-per-week, etc.
- **Target:** Income (<=50K or >50K)

---

## 🛠️ Technologies Used

- Python
- Pandas & NumPy for data handling
- Scikit-learn for preprocessing and metrics
- Matplotlib & Seaborn for visualization

---

## 🧪 Workflow Summary

1. **Data Loading & Cleaning**
   - Load the data from UCI repository
   - Drop missing values and apply label encoding

2. **Preprocessing**
   - Split into training and test sets
   - Standardize features

3. **Modeling**
   - Custom `GaussianNaiveBayes` class that computes priors and likelihoods
   - Predict on test set using Gaussian PDF

4. **Evaluation**
   - Metrics: Accuracy, Precision, Recall, F1 Score
   - Confusion matrix visualization

---

## 📝 Results

- The model shows balanced performance across key metrics for a simple statistical classifier.
- Ideal for learning how Naive Bayes works under the hood with numerical inputs.

---

## 📦 Setup Instructions

1. Clone the repository or copy the script.
2. Install dependencies:

```bash
pip install -r requirements.txt
