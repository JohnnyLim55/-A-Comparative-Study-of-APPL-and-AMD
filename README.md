# Predicting Stock Prices with Long Short-Term Memory Neural Networks: A Comparative Study of AAPL and AMD
## Overview
This project explores the effectiveness of Long Short-Term Memory (LSTM) neural networks in predicting stock prices for two tech giants, Apple Inc. (AAPL) and Advanced Micro Devices, Inc. (AMD). The dataset includes crucial information about each column, with a focus on the "Date" and "Close" columns. The LSTM architecture is designed following specific guidelines to forecast stock prices.
## First Model 
### Steps
#### 1. Data Exploration and Preprocessing
- Objective: Understand and address the time series data problem.
- Actions:
Explore the dataset to grasp the challenges.
Preprocess the data, separating it into input and output with a window size of 5 (from Monday to Friday) and a horizon of 1 (only Monday).
Split the dataset into training (80%), validation (10%), and test sets (10%).
#### 2. Baseline LSTM Architecture
- Objective: Create a baseline architecture with LSTM units (50) and a Perceptron node at the final layer (units=1).
- Details:
Use ReLU as the activation function for LSTM.
#### 3. Optimization of LSTM Architecture
- Objective: Enhance the baseline architecture for optimal performance.
- Modifications:
Adjust architecture based on results from step 2.
Explain the reasoning behind the chosen approach.
Consider adding or removing layers, changing hyperparameters, or utilizing hyperparameter tuning.
#### 4. Evaluation of Model Performance
- Objective: Evaluate the performance of both architectures on the test set.
- Metrics:
Calculate RMSE, MAE, and MAPE.
Provide a detailed explanation of the results.
## Second Model
### Steps
#### 1. Data Preprocessing
- Objective: Separate time series data and split into training, validation, and test sets.
- Details:
Use a window size of 5 (Monday to Friday) and a horizon of 5 (Monday to Friday).
Split the dataset into 80% training, 10% validation, and 10% test sets.
#### 2. Baseline Transformer Architecture
- Objective: Create a baseline architecture following the provided Transformer for Stocks diagram.
- Details:
Utilize one Conv1D layer with ReLU activation for the FEED FORWARD part.
Adjust the Perceptron node in the output based on the horizon.
#### 3. Optimization of Transformer Architecture
- Objective: Modify the baseline Transformer architecture for optimal classification results.
- Modifications:
Adjust the architecture, considering elements like dropout, batch normalization, etc.
Perform hyperparameter tuning for improved performance.
#### 4. Evaluation of Model Performance
- Objective: Evaluate the optimized Transformer architecture's performance on the test set.
- Details:
Provide a detailed evaluation, explaining the obtained results.
