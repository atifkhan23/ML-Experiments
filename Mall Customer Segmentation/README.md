# Project: Mall Customer Segmentation
Description: Add project description here.
# 🛍️ Mall Customer Segmentation using K-Means Clustering

## 📌 Objective

This project focuses on segmenting mall customers into distinct groups based on their demographic and spending patterns. It uses **Unsupervised Machine Learning** — specifically the **K-Means Clustering algorithm** — to group similar customers, which can help with targeted marketing strategies.

---

## 🧾 Dataset Information

- **CustomerID**: Unique identifier for each customer
- **Gender**: Male/Female
- **Age**: Age of the customer
- **Annual Income (k$)**: Annual income in thousands
- **Spending Score (1-100)**: Score assigned by the mall based on customer behavior

- **Source**: Available on [Kaggle](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python)

---

## 🔍 Workflow

### 1. Data Preprocessing & Cleaning
- Check for nulls and types
- Categorical vs numerical feature separation
- Encode categorical values if necessary

### 2. Exploratory Data Analysis (EDA)
- Distribution plots
- Mean analysis using heatmaps
- Insights on Age, Income, and Spending Score

### 3. Feature Engineering
- Selection of relevant features for clustering
- Normalization/Standardization (optional but recommended)

### 4. Modeling
- Apply **K-Means Clustering**
- Use **Elbow Method** and **Silhouette Score** to find optimal `k`
- Visualize clusters in 2D and 3D

### 5. Conclusion
- Summarize findings and recommended segments
- Discuss business implications of each cluster

---

## 💡 What You'll Learn

- How to explore and clean real-world customer data
- Implementing **K-Means Clustering**
- Choosing the best number of clusters (`k`)
- Visualizing high-dimensional cluster data
- Impact of scaling on unsupervised models

---

## 📁 Files

- `mall_segmentation.ipynb` — Main notebook with code and visualizations
- `Mall_Customers.csv` — Input dataset
- `requirements.txt` — Dependencies for easy setup

---

## 🛠️ Setup Instructions

Install the necessary libraries:

```bash
pip install -r requirements.txt
