# deep-learning-challenge
# Alphabet Soup Charity Neural Network Analysis

## Overview

This analysis aims to develop a deep learning model for Alphabet Soup Charity to predict the success of charitable donations. The model utilizes a neural network to classify organizations based on various features.

## Results

### Data Preprocessing

- **Target Variable(s):**
  - `IS_SUCCESSFUL`

- **Feature Variable(s):**
  - All columns except `IS_SUCCESSFUL`, `EIN`, and `NAME`

- **Removed Variables:**
  - `EIN` and `NAME`

### Compiling, Training, and Evaluating the Model

- **Neural Network Architecture:**
  - Number of Layers: 3 (1 input, 2 hidden, 1 output)
  - Number of Neurons:
    - Input Layer: Variable based on the number of features
    - Hidden Layers: 80 (1st layer), 30 (2nd layer)
    - Output Layer: 1 (binary classification)

- **Activation Functions:**
  - Hidden Layers: ReLU
  - Output Layer: Sigmoid (for binary classification)

- **Target Model Performance:**
  - Achieved accuracy: ~72.57%

- **Steps Taken to Improve Performance:**
  - Experimentation with different architectures and activation functions
  - Scaling input data using StandardScaler
  - Training for 100 epochs

## Summary

The deep learning model demonstrated moderate success. However, to enhance performance, it is recommended to explore alternative models, specifically ensemble methods like random forests or gradient boosting. These models could potentially outperform the neural network, especially considering the imbalanced nature of the dataset. Experimenting with feature engineering and hyperparameter tuning may further improve the model's predictive power.
