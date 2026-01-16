# Customer Churn Prediction – Machine Learning Analysis

## Overview
This project focuses on predicting customer churn using supervised machine learning techniques on the Telco Customer Churn dataset. The notebook implements a complete data science workflow including data exploration, preprocessing, class imbalance handling, model training, and evaluation. The goal is to identify customers likely to discontinue a service and understand the factors influencing churn.

## Problem Statement
Customer churn negatively impacts business revenue and growth. This project formulates churn prediction as a binary classification problem and compares multiple machine learning models to identify the most effective approach while maintaining interpretability.

## Dataset
- Dataset: Customer Churn
- Target Variable: Churn
- Target Type: Binary (Yes / No)
- Feature Types: Numerical and Categorical

## Data Exploration
Initial analysis involved:
- Inspecting dataset structure and feature types
- Removing `customerID` as a non-predictive identifier
- Converting `TotalCharges` from object to numeric
- Handling missing or blank values
- Identifying class imbalance in the target variable

## Exploratory Data Analysis (EDA)
EDA was performed to understand customer behavior and feature relationships:
- Distribution analysis of numerical features
- Boxplots to detect skewness and outliers
- Correlation heatmap for numerical variables
- Churn trends across contract types, payment methods, and services

## Data Preprocessing
The preprocessing pipeline includes:
- Encoding categorical variables
- Scaling numerical features
- Separating features and target labels
- Handling class imbalance using SMOTE
- Preventing data leakage by applying preprocessing only on training data

## Models Implemented
The following models were trained and evaluated:
- Logistic Regression
- Random Forest Classifier
- AdaBoost Classifier
- XGBoost Classifier

All models were trained using a consistent preprocessing and resampling pipeline.

## Model Evaluation
Model performance was evaluated using:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

Evaluation emphasized recall and F1-score due to class imbalance.

## Key Observations
- Customer churn data is inherently imbalanced
- Applying SMOTE improves detection of churned customers
- Ensemble and boosting models outperform baseline models
- Consistent preprocessing improves model stability

## Tech Stack
- Programming: Python
- Data Analysis: Pandas, NumPy
- Visualization: Matplotlib, Seaborn
- Machine Learning: Scikit-learn
- Imbalance Handling: SMOTE (imbalanced-learn)
- Boosting: XGBoost

## Project Structure
├── churn_not_churn.ipynb
├── README.md
├── dataset_task1.csv


## Conclusion
This project demonstrates a structured and reproducible machine learning pipeline for customer churn prediction, combining exploratory analysis, preprocessing, imbalance handling, and model comparison to derive meaningful business insights.

