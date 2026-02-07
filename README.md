
<b>Market Sales Prediction</b><br/><br/>

<b>Overview</b><br/>
Predict daily sales for multiple products using historical data with Random Forest Regression.
Helps businesses optimize inventory and make data-driven decisions.<br/><br/>

<b>Dataset</b><br/>
File: market_sales.csv<br/>
Columns:<br/>
date: Date of the sales record<br/>
product_id: Unique identifier for each product<br/>
sales: Number of units sold<br/><br/>

<b>Feature Engineering</b><br/>
1. Date features: year, month, day, weekday, is_weekend<br/>
2. Cyclical encoding for months: month_sin, month_cos<br/>
3. Label encoding for categorical columns<br/><br/>

<b>Preprocessing</b><br/>
- Fill missing numeric values with mean<br/>
- Drop original date column after feature extraction<br/><br/>

<b>Model</b><br/>
Random Forest Regressor<br/>
n_estimators = 300<br/>
max_depth = None<br/>
min_samples_split = 2<br/>
min_samples_leaf = 1<br/>
random_state = 42<br/>
n_jobs = -1<br/><br/>

<b>Evaluation Metrics</b><br/>
MAE (Mean Absolute Error)<br/>
RMSE (Root Mean Squared Error)<br/>
R2 (Coefficient of Determination)<br/><br/>

<b>How to Run</b><br/>
1. Install libraries: pandas, numpy, scikit-learn, matplotlib<br/>
2. Place market_sales.csv in the folder<br/>
3. Run the script
<b>Output</b><br/><br/>
The notebook outputs:<br/>
- Model evaluation metrics in the console<br/>
- Plot of <i>Actual vs Predicted Sales</i> for visual comparison
- Top 10 important features contributing to the prediction<br/>

<b>Requirements</b><br/><br/>
- <b>Python 3.8+</b><br/>
- <b>Libraries:</b><br/>
  <br> pandas,numpy,matplotlib,scikit-learn<br/>
