# Deep-Learning-Challenge
![5e7d53b1a42f1f46ee6a0748](https://github.com/SakinaJaffri/Deep-Learning-Challenge/assets/146900226/24f16ba7-d679-4d6a-815d-928ceef04670)
# Alphabet Soup Funding Prediction

This project focuses on building a neural network-based binary classification model to predict the success of organizations funded by Alphabet Soup, using dataset features. The goal is to analyze over 34,000 organizations and predict the success of future applicants.

## Analysis Overview

- **Objective**: Train and evaluate a model to predict the success (target variable: `IS_SUCCESSFUL`) of Alphabet Soup-funded organizations based on provided dataset features.
  
- **Features Used**:
  - `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS`, `ASK_AMT`.
  
- **Data Preprocessing**:
  - Removed irrelevant columns (`EIN`, `NAME`).
  - Handled rare occurrences in categorical columns (`APPLICATION_TYPE`, `CLASSIFICATION`) by grouping them under 'Others'.
  - Encoded categorical features into numerical using dummy variables.
  - Applied data scaling using `StandardScaler` to normalize the dataset.

## Model Architecture and Results

- **Model Structure**:
  - Typically includes an input layer, hidden layers for processing, and an output layer for predictions.
  
- **Architecture** (Initial Attempt):
  - Input Layer: 80 units (ReLU activation)
  - Hidden Layer: 30 units (ReLU activation)
  - Output Layer: 1 unit (Sigmoid activation)
  - Accuracy: 72.90%
  
- **Optimization Attempts**:
  - Adjusted model architecture, changed activation functions, and utilized PCA.
  - Despite efforts, the model accuracy ranged from 71.70% to 73.64%.
  - Hyperparameter tuning using Keras Tuner did not reach the target accuracy of 75%.

## Summary

The project aimed to predict success for Alphabet Soup-funded organizations with an accuracy goal of 75%. Despite optimization efforts, the model achieved an accuracy of 73.64%. Further refinement and exploration are needed to bridge the gap and improve predictive accuracy.
