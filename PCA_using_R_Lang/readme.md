Gross Margin Analysis with MCA and PCA

Project Overview

This project analyzes a dataset to explore the relationships between categorical variables and the continuous target variable, Gross Margin, using Multiple Correspondence Analysis (MCA) and Principal Component Analysis (PCA). The analysis includes data preprocessing, feature selection, dimensionality reduction, and visualization of results to understand how categorical features impact Gross Margin.

Data set source (https://www.kaggle.com/datasets/atifkhan89/gross-margin-analysis-dataset)
Objectives





Perform MCA to analyze and visualize relationships between categorical variables.



Apply PCA on one-hot encoded categorical features for comparison.



Use ANOVA (F-test) to select the most impactful categorical features on Gross Margin.



Visualize the results, including explained variance, individual distributions, variable relationships, and the impact of selected features on Gross Margin.

Dataset

The dataset used is data_PCA.csv, located in the /kaggle/input/rrrrrrrrrr/ directory. It contains categorical variables (e.g., Pricing_Type, Membership, Customer_Segment, etc.) and a continuous target variable, Gross Margin. Ensure the dataset is accessible in the specified path or update the path in the script as needed.

Prerequisites





R: Version 4.0.0 or higher is recommended.



R Packages: Install the required packages listed in requirements.txt using install.packages() in R.

Installation





Clone or download this repository.



Install the required R packages by running the following command in R:

install.packages(read.table("requirements.txt", header = FALSE)$V1)

Alternatively, manually install each package listed in requirements.txt.

File Structure





analysis.R: The main R script containing the code for data loading, preprocessing, MCA, PCA, feature selection, and visualizations.



requirements.txt: Lists the required R packages.



README.md: This file, providing an overview and instructions for the project.



data_PCA.csv: The input dataset (not included; ensure it is placed in the correct directory).

Usage





Place the data_PCA.csv file in the appropriate directory (e.g., /kaggle/input/rrrrrrrrrr/).



Open the analysis.R script in an R environment (e.g., RStudio or Kaggle).



Update the file path in the script if necessary:

df <- read.csv("path/to/your/data_PCA.csv")



Run the script to perform the analysis and generate visualizations:

source("analysis.R")

Analysis Steps





Data Loading and Preprocessing:





Load the dataset and remove rows with missing Gross Margin values.



Define Gross Margin as the continuous target variable.



Categorical Variable Analysis:





Analyze the impact of categorical variables (e.g., Pricing_Type, Membership) on Gross Margin.



Convert categorical variables to factors for MCA.



One-Hot Encoding and PCA:





Encode categorical variables using one-hot encoding.



Perform PCA on the encoded features to reduce dimensionality.



Feature Selection:





Use ANOVA (F-test) to select the top 5 categorical features based on their impact on Gross Margin.



MCA:





Apply MCA to the categorical variables to explore relationships and reduce dimensionality.



Visualizations:





Generate plots for:





Explained variance (eigenvalues) for MCA and PCA.



Distribution of individuals and variables in the reduced MCA space.



Boxplots showing the impact of the top categorical feature on Gross Margin.



Bar plot of F-test scores for selected features.

Visualizations





Eigenvalues Plot: Shows the variance explained by each MCA/PCA dimension.



Individuals Plot: Displays the distribution of observations in the reduced MCA space.



Variables Plot: Illustrates how categories of each variable are positioned in the reduced MCA space.



Boxplot: Visualizes the distribution of Gross Margin across levels of the top categorical feature.



Feature Importance Bar Plot: Shows the F-test scores for the top 5 categorical features.

Requirements

See requirements.txt for the list of required R packages.

Notes





Ensure the dataset path is correctly specified in the script.



The script assumes the dataset contains the specified categorical columns and Gross Margin. Adjust the categorical_cols vector if the column names differ.



MCA is used for categorical data, while PCA is applied to one-hot encoded data for comparison. PCA is less suitable for categorical data, so MCA is the primary method.

License