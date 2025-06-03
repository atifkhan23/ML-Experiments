Chatbot Text Classification Pipeline

Project Overview

This project implements a text classification pipeline to categorize chatbot responses based on scripted (NLU) responses using TF-IDF vectorization and Logistic Regression. The pipeline includes data loading, preprocessing, exploratory data analysis (EDA), model training with hyperparameter tuning, evaluation, and visualization. It also provides a function to predict categories for new AI-generated responses, with a confidence threshold to flag uncertain predictions for manual review.

dataset source (https://www.kaggle.com/datasets/atifkhan89/chatbot-text-classification-dataset)

Objectives





Load and preprocess chatbot conversation data from an Excel file.



Perform Exploratory Data Analysis (EDA) to understand message lengths, response sources, categories, and temporal trends.



Build a classification model to predict conversation categories based on chatbot responses.



Tune hyperparameters using GridSearchCV to optimize model performance.



Visualize model performance and confidence levels.



Provide a prediction function for new AI-generated responses.

Dataset

The dataset, chatbot_dataset.xlsx, contains chatbot conversation data with the following key columns:





user_message: The user's input message.



chatbot_response: The chatbot's response.



response_source: Indicates the source of the response (e.g., 'NLU' for scripted responses).



categories: The category or intent of the conversation.



intent_name: The specific intent associated with the response.



message_time: Timestamp of the message.

The dataset is located at /kaggle/input/my-classified-project/chatbot_dataset.xlsx. Only responses with response_source = 'NLU' are used for training the classification model.

Prerequisites





Python: Version 3.8 or higher is recommended.



Python Libraries: Install the required libraries listed in requirements.txt using pip install -r requirements.txt.



Dataset: Ensure the chatbot_dataset.xlsx file is accessible in the specified path or update the path in the script.

Installation





Clone or download this repository.



Install the required Python libraries by running:

pip install -r requirements.txt



Ensure the dataset file (chatbot_dataset.xlsx) is available in the specified path or update the path in the script.

File Structure





chatbot_classification.py: The main Python script containing the code for data loading, EDA, preprocessing, model training, evaluation, and visualization.



requirements.txt: Lists the required Python libraries.



README.md: This file, providing an overview and instructions for the project.



chatbot_dataset.xlsx: The input dataset (not included; ensure it is placed in the correct directory).

Usage





Place the chatbot_dataset.xlsx file in the correct directory (e.g., /kaggle/input/my-classified-project/).



Update the file path in the script if necessary:

file_path = "/path/to/chatbot_dataset.xlsx"



Run the script in a Python environment (e.g., Jupyter Notebook, Kaggle, or local IDE):

python chatbot_classification.py



The script will:





Load and preprocess the dataset.



Perform EDA (e.g., message length distributions, response source counts, temporal trends).



Train a Logistic Regression model with TF-IDF vectorization.



Tune hyperparameters using GridSearchCV.



Evaluate the model and visualize performance.



Provide a function to predict categories for new responses.

Analysis Steps





Data Loading and Preprocessing:





Load the dataset from an Excel file and map expected column names dynamically.



Filter for scripted (NLU) responses to ensure consistent training data.



Compute message lengths for user messages and chatbot responses.



Exploratory Data Analysis (EDA):





Visualize message length distributions using histograms.



Plot messages sent per hour and daily trends.



Analyze the distribution of response sources, categories, and top intents.



Generate a correlation matrix for numerical features (if applicable).



Feature Extraction and Model Training:





Use TF-IDF Vectorization with a custom preprocessor (lowercase, remove punctuation) to convert chatbot responses into numerical features.



Train a Logistic Regression model using a scikit-learn pipeline.



Perform hyperparameter tuning with GridSearchCV (e.g., n-gram range, max_df, min_df, regularization strength).



Model Evaluation:





Evaluate the model on a validation set using accuracy, precision, recall, and F1-scores.



Visualize the confusion matrix to analyze classification performance.



Plot the distribution of model confidence scores with a threshold for manual tagging.



Prediction:





Provide a predict_category function to classify new AI-generated responses, flagging low-confidence predictions for manual review.

Visualizations





Histogram: Distribution of user message and chatbot response lengths.



Count Plots: Messages per hour, response sources, and conversation categories.



Line Plot: Number of messages per day.



Bar Plot: Top 10 most common intents.



Heatmap: Correlation matrix for numerical features (if applicable).



Confusion Matrix Heatmap: Model performance on the validation set.



Histogram: Distribution of model confidence scores with a threshold line.

Requirements

See requirements.txt for the list of required Python libraries.

Notes





Ensure the dataset path and column names are correctly specified in the script.



The script dynamically maps column names to handle variations in naming conventions.



Only scripted (NLU) responses are used for training to ensure consistency.



The prediction function includes a confidence threshold (default 0.6) to flag uncertain predictions for manual tagging.



The script is optimized for a Kaggle environment but can be adapted for local use by updating the dataset path.