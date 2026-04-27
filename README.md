# Credit-card-fraud-detection-system

This repository contains a machine learning project focused on detecting fraudulent credit card transactions. The system addresses the significant challenge of class imbalance inherent in fraud detection datasets, where legitimate transactions vastly outnumber fraudulent ones.

## Key Features:

*   **Data Loading and Preprocessing**: Efficiently loads and prepares credit card transaction data, including feature engineering for 'Time' and 'Amount' features.
  
*   **Class Imbalance Handling**: Utilizes **SMOTE (Synthetic Minority Oversampling Technique)** to balance the training dataset, preventing models from being biased towards the majority class.

  
*   **Model Training and Optimization**: Implements and tunes various classification models, with a strong emphasis on **XGBoost** for its performance in tabular data. Hyperparameter optimization is performed using `RandomizedSearchCV` for Random Forest and `Optuna` for XGBoost.
  
*   **Ensemble Modeling**: Incorporates a Voting Ensemble approach to combine predictions from multiple models (Logistic Regression, Random Forest, XGBoost) for improved robustness and performance.
  
*   **Automated Machine Learning (AutoML)**: Explores an AutoML-like pipeline search to identify effective model configurations.
  
*   **Comprehensive Evaluation**: Focuses on appropriate metrics for imbalanced datasets, such as Precision, Recall, F1-Score, ROC-AUC, and **Average Precision (PR-AUC)**, which is crucial for fraud detection.
  
*   **Visualizations**: Generates insightful plots including ROC curves, Precision-Recall curves, confusion matrices, and feature importance to provide a clear understanding of model performance and drivers.

## Models Explored:

*   Logistic Regression (Baseline)
  
*   Tuned Random Forest
  
*   Tuned XGBoost (optimized with Optuna)
  
*   Voting Ensemble
  
*   AutoML Best Pipeline

This system aims to achieve a high recall for fraud detection while maintaining acceptable precision, thereby minimizing financial losses due to fraud.
