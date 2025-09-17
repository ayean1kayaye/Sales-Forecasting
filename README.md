# Sales-Forecasting
This repository forecasts sales quantities of warehouse inventory for beauty products, leveraging a robust time series dataset and regression-based machine learning models. The main goal is to predict weekly sales for the next 13 weeks and identify the most effective regression model for this time series forecasting challenge


Objectives

	•	Forecast warehouse stock sales for the upcoming 13 weeks using historical weekly sales data .
	•	Evaluate whether future sales are trending upward or downward, based on predictions and time series trend analysis .
	•	Compare multiple regression models to select the best one for accurate time series stock prediction, using metrics such as Mean Absolute Error (MAE) 


Methodology

	•	Exploratory Data Analysis (EDA): Assessed sales distribution, trends, and seasonality at weekly and monthly levels. Detected and visualized upward and downward trends using polynomial fitting and time series decomposition .
	•	Feature Engineering: Grouped and resampled data by weekly intervals, extracted date features (year, month, weekday) .
	•	Modeling: Compared several regression models for time series forecasting:
	•	Linear Regression
	•	Random Forest Regressor
	•	Gradient Boosting Regressor
	•	XGBoost Regressor
	•	Hyperparameter Tuning: Utilized GridSearchCV for each model to select optimal hyperparameters .
	•	Evaluation: Trained and tested each model, measured performance using Mean Absolute Error (MAE), visualized actual vs predicted trends .


Results

	•	All tested regression models provided reasonably robust predictions for stock sales .
	•	Gradient Boosting Regressor achieved the lowest test MAE among all models, indicating the highest forecasting accuracy on unseen weeks .
	•	The predicted sales for the next 13 weeks show observable temporal patterns, with slight fluctuations and periodic behavior depending on the chosen model .

 
Usage

Clone this repository and run the notebook to:

	•	Preprocess new data
	•	Compare regression models for time series forecasting
	•	Visualize and interpret warehouse sales trends and forecasts for the next 13 weeks 

 
Project Structure

	•	`data/` — Contains the input timeseries CSV file
	•	`notebooks/` — Jupyter notebook for end-to-end analysis and modeling
	•	`outputs/` — Plots and visualizations of sales trends and model forecasts

