# Project: gradient_decent (2)
Description: Add project description here.
# Gradient Descent Sensitivity to Feature Scaling

## 📌 Overview

This project demonstrates how **feature scaling** affects the performance of **gradient descent optimization**. By using synthetic data with features on vastly different scales, we visualize how convergence speed varies before and after scaling.

## 📊 Objectives

- Simulate a dataset with small and large scale features
- Apply gradient descent on:
  - Unscaled data
  - Min-Max scaled data
  - Separately scaled features
- Compare convergence behavior via cost (MSE) plots

---

## 🧪 Techniques Used

- **Manual Gradient Descent** implementation (no libraries like sklearn used for training)
- **Min-Max Scaling** and **Standard Scaling** via `sklearn.preprocessing`
- Cost history plotted with `matplotlib`

---

## 📁 Files

- `gradient_descent_scaling_comparison.py` (main script)
- `requirements.txt` (dependencies)

---

## 🔧 Installation

Create a virtual environment and install dependencies:

```bash
pip install -r requirements.txt
