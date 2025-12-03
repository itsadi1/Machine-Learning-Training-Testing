# AI Developer Performance Predictor: Regression Analysis
A machine learning project that analyzes factors influencing AI developer performance and utilizes a Gradient Boosting Regressor to predict the Task Success Rate.

## Project Overview
The primary goal of this project is to build a regression model capable of predicting an AI developer's Task Success Rate based on various productivity, health, and environmental factors.

The key steps involved in this analysis include:

+ Data loading and initial exploration.
+ Checking for missing values and data types.
+ Visualizing feature correlation using a Correlation Matrix.
+ Splitting data into training and testing sets.
+ Training a Gradient Boosting Regressor.
+ Evaluating the model using standard regression metrics.

The project utilizes the `AI_Developer_Performance_Extended_1000.csv` dataset, sourced from the "ai-dev-performance" dataset on Kaggle.

The dataset contains **1000 data points** and **13 features**.

## Features

The features included in the dataset are:

- `Hours_Coding`
- `Lines_of_Code`
- `Bugs_Found`
- `Bugs_Fixed`
- `AI_Usage_Hours`
- `Sleep_Hours`
- `Cognitive_Load`
- `Task_Success_Rate` (**Target Variable**)
- `Coffee_Intake`
- `Stress_Level`
- `Task_Duration_Hours`
- `Commits`
- `Errors`

## Methodology

### Model Selection

A **GradientBoostingRegressor** was chosen for its robustness and performance in capturing complex non-linear relationships within the dataset.

### Evaluation Metrics

The model's performance was assessed using the following metrics:

- **R² Score (Coefficient of Determination)**: Measures the proportion of the variance in the dependent variable that is predictable from the independent variables.
    
- **Mean Absolute Error (MAE)**: The average of the absolute differences between predictions and actual values.
    
- **Mean Squared Error (MSE)**: The average of the squares of the errors.
    
- **Root Mean Squared Error (RMSE)**: The square root of the MSE, providing an error measure in the same units as the target variable.

## Performance Results

The **GradientBoostingRegressor** achieved the following results on the test set:

|**Metric**|**Value**|
|---|---|
|**Accuracy (GBR Score)**|0.95|
|**R² Score**|0.95|
|**Mean Absolute Error (MAE)**|3.72|
|**Mean Squared Error (MSE)**|21.62|
|**Root Mean Squared Error (RMSE)**|4.65|

_The R² score of **0.95** suggests that the model is able to explain 95% of the variance in the `Task_Success_Rate`._
