# Predicting Nifty 50 Index Prices

## Overview
This project aims to predict daily prices of the Nifty 50 index using machine learning techniques. The Nifty 50 index represents the performance of India’s top 50 companies listed on the National Stock Exchange (NSE). By leveraging historical data and advanced modeling approaches, the project seeks to provide accurate forecasts essential for financial decision-making.

## Dataset
- The dataset used contains daily historical data including open, high, low, and close prices of the Nifty 50 index.
- Additional features include financial ratios such as P/E ratio, P/B ratio, and dividend yield percentage.
- Date columns were transformed into datetime format, and missing values were handled appropriately during preprocessing.

## Features
- **Date Features:** Extracted year, quarter, month, and day from the date column to enrich the dataset.
- **Transformation:** Applied log transformation to stabilize variance and standardization to financial ratios for consistent scaling.

## Modeling
- Explored various machine learning algorithms including:
  - Linear Regression
  - Lasso Regression
  - Ridge Regression
  - Gradient Boosting Regressor
  - XGBoost Regressor
- Evaluated models using metrics such as Mean Squared Error (MSE) and Root Mean Squared Error (RMSE).
- Selected the Gradient Boosting Regressor as the best-performing model based on evaluation metrics.

## Deployment
- Saved the final model (`best_model.pkl` or `best_model.joblib`) using Python's `pickle` or `joblib` libraries for future deployment.
- Ensure compatibility with the deployment environment and implement security protocols for handling serialized models.

## Project Structure
```
├── data/                    # Directory for storing dataset
│   ├── nifty50_data.csv     # Raw dataset file
├── models/                  # Directory for storing trained models
│   ├── best_model.pkl       # Serialized model file
├── notebooks/               # Directory for Jupyter notebooks (if applicable)
│   ├── EDA.ipynb            # Exploratory Data Analysis notebook
│   ├── Modeling.ipynb       # Model development and evaluation notebook
├── src/                     # Directory for source code (if applicable)
│   ├── data_preprocessing.py   # Script for data preprocessing
│   ├── model_training.py       # Script for model training and evaluation
├── README.md                # Project overview and instructions
└── requirements.txt         # Python dependencies

```
