# Alphabet Soup Funding Prediction - Deep Learning Challenge

![Alphabet Soup](https://github.com/SakinaJaffri/Deep-Learning-Challenge/assets/146900226/24f16ba7-d679-4d6a-815d-928ceef04670)

## Overview

This project involves building a neural network model to predict the success of organizations funded by **Alphabet Soup**. Using a dataset of over 34,000 funded organizations, the goal is to develop a binary classification model that can accurately predict whether future funding applications will be successful based on a set of features.

## Objective

- **Target**: Predict the `IS_SUCCESSFUL` variable (success or failure) based on organization details.
- **Features**: 
  - `APPLICATION_TYPE`, `AFFILIATION`, `CLASSIFICATION`, `USE_CASE`, `ORGANIZATION`, `STATUS`, `INCOME_AMT`, `SPECIAL_CONSIDERATIONS`, `ASK_AMT`
- **Excluded Columns**: `EIN`, `NAME`

## Data Preprocessing

- **Cleaning**: Dropped unnecessary columns (`EIN`, `NAME`).
- **Feature Engineering**: Grouped rare categories in `APPLICATION_TYPE` and `CLASSIFICATION` into an "Others" category.
- **Encoding**: Categorical features were converted into numerical dummy variables.
- **Scaling**: Applied `StandardScaler` to normalize the data.

## Model Architecture

- **Neural Network Model**: 
  - Input, hidden, and output layers designed for binary classification.
  - Different configurations of layer sizes and activation functions were tested.
  
- **Optimization**:
  - Experimented with multiple architectures and used `keras-tuner` to improve model performance.
  - Principal Component Analysis (PCA) was used to reduce dimensionality in certain trials.

## Results

- **Initial Model**: Achieved an accuracy of 72.54%.
- **Optimized Model**: Maximum accuracy of 73.30% after hyperparameter tuning and experimentation.
- **Target**: While the goal was to achieve 75% accuracy, further improvements are required to meet this threshold.

## Summary

Despite extensive efforts in preprocessing, feature engineering, and model optimization, the highest accuracy achieved was 73.30%. The project highlights the complexities of predicting the success of funded organizations and suggests room for further refinement and exploration to improve model accuracy.

## Technologies Used

- **Python**
- **TensorFlow/Keras**
- **Pandas**
- **Scikit-learn**
- **Jupyter Notebook**

## How to Run

1. Clone the repository to your local machine.
2. Install the required dependencies listed in `requirements.txt`.
3. Run the Jupyter Notebook to preprocess the data and train the model.
4. Experiment with different neural network architectures and optimizations.

## Contributors

- **Sakina Jaffri** - Project Developer
