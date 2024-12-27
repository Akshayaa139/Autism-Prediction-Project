# Autism-Prediction-Project


This project leverages machine learning algorithms to predict autism spectrum disorder (ASD) based on input features. The primary goal is to provide a tool that can assist healthcare professionals in early identification of autism traits, potentially facilitating timely interventions.

Table of Contents
Introduction
Features
Data
Modeling Approach
Setup and Installation
Usage
Results
Future Enhancements
Contributors
License
Introduction
Autism spectrum disorder (ASD) is a developmental condition that affects communication, behavior, and social interaction. Early diagnosis is crucial for effective intervention. This project aims to predict ASD based on key indicators using machine learning techniques.

Features
Data Preprocessing: Handles missing values, categorical encoding, and data normalization.
Imbalanced Data Handling: Utilizes SMOTE (Synthetic Minority Over-sampling Technique) to balance the dataset.
Model Training: Implements multiple classifiers, including:
Decision Tree
Random Forest
XGBoost
Hyperparameter Tuning: Uses RandomizedSearchCV for optimal model configuration.
Evaluation Metrics: Employs accuracy, precision, recall, and F1-score to evaluate model performance.
Data
The dataset used in this project includes various features that assess:

Social behaviors
Communication patterns
Repetitive actions
Cognitive abilities


Preprocessing Steps:

Handled missing values.
Applied SMOTE for class balancing.
Normalized numerical features.
Modeling Approach
Exploratory Data Analysis (EDA): Insights into feature distributions and correlations.
Feature Engineering: Selected key features contributing to ASD prediction.
Model Selection: Compared multiple machine learning algorithms.
Evaluation: Assessed model performance using cross-validation.

Results
Accuracy Score: 81.88%
The model correctly predicted outcomes approximately 81.88% of the time on the test dataset.

Confusion Matrix:



[[108  16]
 [ 13  23]]
True Negatives (108): Correctly identified non-autism traits.
False Positives (16): Misclassified non-autism traits as autism traits.
False Negatives (13): Misclassified autism traits as non-autism traits.
True Positives (23): Correctly identified autism traits.
Classification Report:

Class 0 (Non-Autism Traits):
Precision: 0.89
Recall: 0.87
F1-Score: 0.88
Class 1 (Autism Traits):
Precision: 0.59
Recall: 0.64
F1-Score: 0.61
Macro Average:

Precision: 0.74
Recall: 0.75
F1-Score: 0.75
Weighted Average:

Precision: 0.82
Recall: 0.82
F1-Score: 0.82
The model demonstrates strong performance in predicting non-autism traits but shows potential for improvement in identifying autism traits accurately.

