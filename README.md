
<b>AIML_Project</b><br/><br/>

<b>Market Sales Prediction using Random Forest</b><br/><br/>

<b>Project Overview</b><br/>
This project predicts daily sales for multiple products using historical sales data and time-based features. 
The model uses Random Forest Regression to forecast sales, allowing businesses to optimize inventory, 
plan marketing campaigns, and make data-driven decisions.<br/><br/>

<b>Dataset</b><br/>
File: market_sales.csv<br/>
Columns:<br/>
date: Date of the sales record<br/>
product_id: Unique identifier for each product<br/>
sales: Number of units sold<br/><br/>

<b>Features</b><br/>
Time-based features: year, month, day, weekday, is_weekend<br/>
Seasonal features: month_sin, month_cos<br/>
Lag features: lag_1, lag_7, lag_14<br/><br/>

<b>Product Encoding</b><br/>
product_id is one-hot encoded to handle categorical values.<br/><br/>

<b>Model</b><br/>
Algorithm: Random Forest Regressor<br/>
Hyperparameters: n_estimators=400, max_depth=10, min_samples_split=2, 
min_samples_leaf=1, random_state=42, n_jobs=-1<br/>
Train-test split: 80/20<br/><br/>

<b>Performance Metrics</b><br/>
MAE, RMSE, R² Score<br/><br/>

<b>Visualization</b><br/>
Actual vs Predicted Sales (first 150 time steps)<br/><br/>

<b>Requirements</b><br/>
Python 3.8+, pandas, numpy, matplotlib, scikit-learn<br/><br/>

<b>Usage</b><br/>
Place market_sales.csv in the project folder and run:<br/>
python sales_prediction.py<br/><br/>

<b>Output</b><br/>
Model evaluation metrics and a plot of actual vs predicted sales.
"""

content.append(Paragraph(text, styles["Normal"]))
doc.build(content)

file_path

