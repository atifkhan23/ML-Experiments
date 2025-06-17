# Project: califoenia_house_prediction
Description: Add project description here.
# California Housing Price Prediction

## Overview
This project uses the **California housing dataset** to predict **median house values** based on various features such as location, number of rooms, population, income, and proximity to the ocean.

## Dataset Summary
- **Entries**: 20,640
- **Features**:
  - `longitude`, `latitude`
  - `housing_median_age`
  - `total_rooms`, `total_bedrooms`
  - `population`, `households`
  - `median_income`
  - `median_house_value` (target)
  - `ocean_proximity` (categorical)

## Key Tasks

### 1. Data Inspection
- Identified that `total_bedrooms` has 207 missing values.
- Data types: 9 numerical features and 1 categorical (`ocean_proximity`).

### 2. Exploratory Data Analysis (EDA)
- Bar plots and value counts used to analyze `ocean_proximity` distribution.
- Checked for label imbalance and missing data.
- Examined value distributions and relationships between features.

### 3. Handling Missing Data
- Used strategies such as **mean imputation** or **median** for missing `total_bedrooms`.

### 4. Model Preparation (Next Steps)
- Convert categorical variables using one-hot encoding.
- Normalize features.
- Apply regression models like **Linear Regression**, **Random Forest**, or **Gradient Boosting**.

## Feature Types

| Feature               | Type     |
|-----------------------|----------|
| longitude             | float64  |
| latitude              | float64  |
| housing_median_age    | float64  |
| total_rooms           | float64  |
| total_bedrooms        | float64 (has missing values) |
| population            | float64  |
| households            | float64  |
| median_income         | float64  |
| median_house_value    | float64 (Target) |
| ocean_proximity       | object (Categorical) |

## Next Steps
- Model training & hyperparameter tuning
- Feature engineering (e.g., room-per-household ratios)
- Evaluate using RMSE, MAE, R²
- Deploy as a web service or dashboard

 