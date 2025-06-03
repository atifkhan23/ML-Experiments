Patient Visit Forecasting Project (2019–2021)

Overview

This project performs time series forecasting on weekly patient visit data from 2019 to 2021, utilizing both statistical and machine learning models. The goal is to predict future patient visits and compare model performance using accuracy metrics such as RMSE, MAE, and MAPE. The analysis includes exploratory data analysis (EDA) to uncover trends and seasonality, model training, forecasting, and visualization of results.

Requirements



Dataset source : ("https://www.kaggle.com/datasets/atifkhan89/cvs-covid-forecasting-data-20192021")

Python Libraries:





numpy, pandas for data processing



matplotlib, seaborn for visualization



statsmodels for statistical models (Holt-Winters, ARIMA, SARIMA)



scikit-learn for machine learning models (Random Forest, Gradient Boosting, Linear Regression, SVR, KNN, Decision Tree, AdaBoost)



xgboost (optional, for XGBoost model)



Dataset:





Excel file: CVS_COVID_Forecasting_Data_2019_2021_With_Locations_Staff.xlsx



Contains weekly patient visit data with columns for Year, Week, Patient_Visits, and Staff_Count



Environment: Designed to run in Jupyter or Kaggle environments with flexible file path handling

Project Structure





Data Loading:





Loads the dataset from specified paths (Kaggle or local).



Handles missing file errors gracefully.



Preprocessing:





Sorts data by Year and Week.



Creates a Time_Index with weekly frequency starting from January 1, 2019.



Sets Time_Index as the DataFrame index and extracts Patient_Visits for forecasting.



Exploratory Data Analysis (EDA):





Trend Line: Visualizes weekly patient visits to detect trends.



Distribution Histogram: Shows the distribution of visit counts.



Staff vs. Visits Correlation: Scatterplot to analyze the relationship between staff count and visits.



Average Visits by Week Number: Highlights seasonal patterns across weeks.



Monthly Boxplot: Displays month-wise variation in visits to capture seasonality.



Train/Test Split:





Splits data into training (all but last 12 weeks) and testing (last 12 weeks) sets.



Converts week indices into numeric format for machine learning models.



Model Training and Forecasting:





Statistical Models:





Holt-Winters (Triple Exponential Smoothing, additive trend/seasonality, 52-week period)



ARIMA(2,1,2) for trend and short-term dependencies



SARIMA(1,1,1)(1,1,1,52) for trend and weekly seasonality



Machine Learning Models:





Random Forest



Gradient Boosting



XGBoost (if available)



Linear Regression



Support Vector Regressor (SVR)



K-Nearest Neighbors (KNN)



Decision Tree



AdaBoost



Models are trained on numeric week indices and forecast the test period (12 weeks).



Evaluation Metrics:





Computes RMSE, MAE, and MAPE for each model's predictions.



Compares performance across all models.



Visualization:





Plots actual vs. predicted patient visits for all models in a single color-coded graph.



Results Summary:





Displays a table of accuracy metrics (RMSE, MAE, MAPE) sorted by RMSE.



Recommends the model with the lowest RMSE.

How to Run





Install Dependencies:

pip install numpy pandas matplotlib seaborn statsmodels scikit-learn xgboost

Note: xgboost is optional; the code checks for its availability.



Prepare Dataset:





Place the Excel file (CVS_COVID_Forecasting_Data_2019_2021_With_Locations_Staff.xlsx) in one of the specified paths:





Kaggle: /kaggle/input/covide-dataset/



Local: /mnt/data/



Update file_paths in the code if using a different location.



Run the Notebook:





Execute the Jupyter notebook or Python script in a compatible environment (e.g., Jupyter, Kaggle).



Ensure all required libraries are installed.



Outputs:





EDA Plots: Trend, distribution, staff correlation, weekly averages, and monthly boxplots.



Forecast Plot: Comparison of actual vs. predicted visits for all models.



Accuracy Table: Metrics (RMSE, MAE, MAPE) for each model.



Recommendation: The model with the lowest RMSE is highlighted.

Notes





The dataset must include Year, Week, Patient_Visits, and Staff_Count columns.



The code is designed to handle missing xgboost gracefully; if unavailable, XGBoost is skipped.



Adjust model parameters (e.g., ARIMA/SARIMA orders, ML hyperparameters) as needed for specific use cases.



Visualizations are optimized for clarity with proper labels, legends, and gridlines.