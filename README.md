# DemandEdge: Forecasting Product Demand with Advanced Models

This repository contains the implementation of the **DemandEdge** project, a comprehensive system for forecasting product demand using advanced time series and machine learning models. The primary goal is to predict demand with high accuracy while analyzing historical trends, product categories, and seasonal patterns.

## Key Features

- **Data Preparation and Cleaning:** Handles noisy and complex datasets with thorough preprocessing.
- **Forecasting Models:** Utilizes SARIMA, ARIMA, and XGBoost for accurate demand prediction.
- **Evaluation Metrics:** SMAPE (Symmetric Mean Absolute Percentage Error) is the primary metric for evaluation, ensuring balanced assessment across datasets.
- **Visualization Tools:** Provides detailed plots for exploratory data analysis (EDA) and model performance insights.

## Notebook Overview

### `demandEdge_notebook.ipynb`

This Jupyter notebook is the main implementation file for the project. It includes:

1. **Data Import and Preprocessing**:
    - Loading historical demand data.
    - Handling missing values and encoding categorical variables.
2. **Exploratory Data Analysis (EDA)**:
    - Visualizing demand trends, seasonality, and product category insights.
3. **Model Implementation**:
    - SARIMA and ARIMA for time series analysis.
    - XGBoost for incorporating additional features.
4. **Forecast Generation**:
    - Step-by-step creation of demand forecasts.
5. **Evaluation**:
    - Calculation of SMAPE and other error metrics.
6. **Visualization**:
    - Comparing predicted vs. actual demand.

## Evaluation Metric

**SMAPE (Symmetric Mean Absolute Percentage Error):**

![SMAPE Formula](https://latex.codecogs.com/png.latex?SMAPE%20%3D%20%5Cfrac%7B100%25%7D%7Bn%7D%20%5Csum_%7Bt%3D1%7D%5E%7Bn%7D%20%5Cfrac%7B%7CF_t%20-%20A_t%7C%7D%7B(%7CA_t%7C%20%2B%20%7CF_t%7C)%2F2%7D)

Where:
- \( F_t \): Forecasted value  
- \( A_t \): Actual value  

**Special Case**: SMAPE is defined as 0 when both actual and predicted values are 0.


## Acknowledgements
- Forecasting Models: SARIMA, ARIMA, XGBoost
- Evaluation Support: SMAPE metric development and testing
