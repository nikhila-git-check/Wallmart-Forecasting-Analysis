# Walmart Store Sales Forecasting 
– Initial EDA & Baseline Model

## Overview

This project forecasts weekly product sales for Walmart stores using historical sales data and external factors such as holidays, promotions, and economic indicators. 
The goal is to build a regression model that helps improve inventory planning, promotion timing and resource allocation.

## Problem Statement

Can we use seasonal patterns and historical data to forecast future product sales in order to improve business strategy?

Accurate sales prediction is critical for avoiding stockouts and overstock situations, reducing waste, and supporting data-driven decisions for supply chain and marketing.

## Data

The dataset comes from the Kaggle competition **"Walmart Sales Forecasting dataset"** and includes:
- Historical weekly sales at the Store–Department level
- Store characteristics (Type, Size)
- External features such as:
  - Temperature
  - Fuel price
  - Consumer Price Index (CPI)
  - Unemployment
  - Promotional markdowns
  - Holiday flags

## Methods

In this initial module, I focused on:
- Data cleaning (handling missing values, checking duplicates)
- Feature engineering:
  - Date-based features (Year, Month, WeekOfYear)
  - Lagged sales features
  - Encoded store type and holiday indicators
- Exploratory data analysis (EDA):
  - Time series plots of weekly sales
  - Distributions of key variables
  - Holiday vs non-holiday comparisons
  - Correlation analysis
- Baseline modeling:
  - Model: RandomForestRegressor
  - Target: Weekly_Sales
  - Metrics: RMSE and R² on a validation set

## Key Findings 

- Weekly sales show strong seasonal/holiday patterns.
- Promotional markdowns and store characteristics (Type, Size) are important predictors of sales.
- The baseline Random Forest model achieves an RMSE of **5063.05** and an R² of **0.94**, providing a reasonable starting point for more advanced modeling.

## Files

- `Wallmart_Sale_Forecasting.ipynb` – Main notebook with data cleaning, EDA, feature engineering, and baseline model.
- `data/` – Contains the raw CSV files from Kaggle

## Next Steps

In the next module, I plan to:
- Add more advanced models (e.g., Gradient Boosting, XGBoost)
- Perform hyperparameter tuning
- Engineer additional time-series and holiday-related features
- Refine visualizations and explanations for both technical and non-technical audiences.
