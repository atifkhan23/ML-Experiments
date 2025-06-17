# Project: Bad_words_detection_using_ml
Description: Add project description here.
# Toxic Comment Classification - Model Evaluation and Insights

## Overview
This project tackles the problem of **multi-label classification** for detecting toxic language in online comments. Each comment may have multiple labels assigned from the following categories:

- toxic
- severe_toxic
- obscene
- threat
- insult
- identity_hate

The dataset used is from the **Jigsaw Toxic Comment Classification Challenge**.

## Objectives
- Perform exploratory data analysis (EDA) on label distribution and correlations.
- Clean and vectorize text data using TF-IDF with bigrams.
- Train and evaluate Logistic Regression, Random Forest, and LightGBM models.
- Implement ensemble voting to combine model outputs.
- Evaluate performance using Precision, Recall, F1-score, and ROC AUC.

## Key Highlights
- Strong AUC scores across most labels, especially using LightGBM and Ensemble Voting.
- Clear performance challenges for rare labels like `threat` and `identity_hate`.
- Potential improvements include class imbalance handling and transformer-based models.

## Folder Structure
