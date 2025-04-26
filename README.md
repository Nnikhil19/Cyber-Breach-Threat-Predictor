This repository contains Python code implementing a machine learning pipeline to predict the impact level of data breaches.

**Goal:** To identify factors associated with "High Impact" breaches, defined as those exceeding a specified record count threshold (e.g., 500,000). Uses breach size as a proxy for overall impact due to data constraints.

**Features:**
*   Loads data breach records from a CSV file.
*   Performs data cleaning and preprocessing (imputation, scaling, one-hot encoding).
*   Creates a binary target variable based on the `breach_size` threshold.
*   Splits data into training and testing sets.
*   Trains a `RandomForestClassifier` using `scikit-learn`, employing balanced class weights to handle data imbalance.
*   Evaluates the model using Accuracy, Classification Report, and Confusion Matrix (including plot).
*   Calculates and displays feature importances using `tabulate`.
*   Includes an interactive loop allowing users to input new breach data for prediction.

**Libraries:** `pandas`, `numpy`, `scikit-learn`, `matplotlib`, `tabulate`
