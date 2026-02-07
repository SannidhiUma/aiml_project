# aiml_project
AIML_Project
Market Sales Prediction using Random Forest
Project Overview

This project predicts daily sales for multiple products using historical sales data and time-based features. The model uses Random Forest Regression to forecast sales, allowing businesses to optimize inventory, plan marketing campaigns, and make data-driven decisions.

Dataset

File: market_sales.csv

Columns:

date: Date of the sales record

product_id: Unique identifier for each product

sales: Number of units sold

The dataset contains historical sales data for multiple products over time.

Features

The following features are generated for model training:

Time-based features

year

month

day

weekday

is_weekend: Binary flag for weekends

Seasonal features

month_sin

month_cos: Cyclical encoding of months to capture seasonality

Lag features

lag_1: Sales of the previous day

lag_7: Sales of 7 days ago

lag_14: Sales of 14 days ago

Product Encoding

product_id is one-hot encoded to handle categorical values.

Model

Algorithm: Random Forest Regressor

Hyperparameters:

n_estimators = 400

max_depth = 10

min_samples_split = 2

min_samples_leaf = 1

random_state = 42

n_jobs = -1

Trained using an 80/20 train-test split.

Performance Metrics

MAE (Mean Absolute Error)

RMSE (Root Mean Squared Error)

R² Score (Coefficient of Determination)

Metrics are printed in the console after execution.

Visualization

Actual vs Predicted Sales

First 150 time steps plotted for comparison.

Requirements

Python 3.8+

pandas

numpy

matplotlib

scikit-learn
