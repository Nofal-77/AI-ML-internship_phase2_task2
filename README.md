# Customer Churn Prediction using Machine Learning Pipeline

## Objective  
The objective of this project is to build a machine learning model to predict whether a customer will churn (leave the service) based on their demographic and service usage data.

## Dataset  
The dataset used is the Telco Customer Churn Dataset, which contains customer information such as demographics (e.g., gender, tenure), services subscribed, billing details, and a target variable indicating whether the customer has churned (Yes/No).

## Methodology  
The data preprocessing step involves converting the TotalCharges column to a numeric format and handling missing values appropriately. The target variable (Churn) is transformed into a binary format for model training. Features are separated into numerical and categorical types.

A data transformation pipeline is created where numerical features are processed by imputing missing values using the median and applying standard scaling, while categorical features are handled by imputing missing values and applying one-hot encoding. These transformations are combined using a ColumnTransformer.

A complete machine learning pipeline is then built by integrating the preprocessing steps with a Random Forest Classifier. The dataset is split into training and testing sets in an 80/20 ratio, and the model is trained using this pipeline to ensure a clean and reproducible workflow.

## Evaluation Metrics  
The model is evaluated using a classification report, which includes precision, recall, and F1-score, along with a confusion matrix to assess prediction performance.

## Outcome  
The model is able to effectively predict customer churn using a structured pipeline, demonstrating how preprocessing and model training can be combined into a single workflow for solving real-world classification problems.
