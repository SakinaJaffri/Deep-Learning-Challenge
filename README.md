# Deep-Learning-Challenge
![5e7d53b1a42f1f46ee6a0748](https://github.com/SakinaJaffri/Deep-Learning-Challenge/assets/146900226/24f16ba7-d679-4d6a-815d-928ceef04670)
# Alphabet Soup Funding Prediction

## Overview

This project involves building a neural network model for binary classification to predict the success of organizations funded by Alphabet Soup based on given features in the dataset. The aim is to analyze a dataset of over 34,000 funded organizations and use machine learning techniques, including neural networks, to predict the success of future applicants.

## Analysis Details

- **Objective**: Train and evaluate a model to predict the success of Alphabet Soup-funded organizations using historical data.
  
- **Features and Target Variables**:
  - **Target Variable**: `IS_SUCCESSFUL` (success or failure)
  - **Features**: `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS`, `ASK_AMT`
  - **Excluded**: `EIN` and `NAME` (neither target nor features)

## Data Preprocessing

- **Data Cleaning**:
  - Read CSV data into a Pandas DataFrame.
  - Drop irrelevant columns (`EIN`, `NAME`).

- **Feature Engineering**:
  - Group rare occurrences in `APPLICATION_TYPE` and `CLASSIFICATION` into an "Others" category.
  - Convert categorical features into dummy variables for numerical representation.
  - Scale the data using `StandardScaler` for normalization.

- **Optimization**:
  - Utilize PCA to reduce dimensionality and optimize the model's complexity.
  - Experiment with different feature sets and preprocessing techniques.

## Model Architecture and Results

- **Model Structure**:
  - Neural network with input, hidden, and output layers.
  - Various configurations of layer sizes, activation functions, and units.

- **Results**:
  - Initial model achieved an accuracy of 72.54%.
  - Optimization attempts:
    - Experimented with different layer sizes and activation functions.
    - Used `keras-tuner` to optimize architecture but achieved a maximum accuracy of 73.30%, falling short of the 75% target.

## Summary

Despite rigorous optimization efforts, including adjusting model architectures and hyperparameter tuning, the achieved accuracy of 73.30% underscores the challenge of accurately predicting success for Alphabet Soup-funded organizations. Further refinement and exploration may be needed to bridge the gap and improve predictive performance.

