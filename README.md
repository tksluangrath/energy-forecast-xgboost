# AEP Energy Forecasting with XGBoost

## Project Overview

Forecast hourly electricity demand (MW) for American Eletric Power using XGBoost, a powerful gradient boosting algorithm. 

## Project Goal

Beyond predicting energy consumption, this project aims to deepen understanding of the XGBoost algorithm on Python. Some concepts would be its strength, hyperparatmeter tuning stratgies, and limiations whe applied to time-dependent data. The objective is to iteratively refine the model to improve accuracy, interpretability, and generalization on unseen data.

## Dataset

- Source: AEP hourly energy consumption
- Units: Megawatts (MW) 
- Range: 2004-10-01 01:00:00 to 2018-08-03 00:00:00

## Methods

- Time Series Split (Train/Test on 2015 threshold)
- Feature Engineering: Hour, Day of Week, Month, etc.
- XGBoost Regression Model
- Evaluation using RMSE

## Key Results

RMSE Score on Test set: 1644.3873

Worst Predicted:
```
2017-01-22    4872.108968
2015-02-20    4861.401571
2015-02-19    4769.359985
2018-01-06    4403.549683
2017-02-07    4290.881022
```

Best Predicted:
```
2017-12-24    222.424520
2016-12-13    236.145426
2017-03-18    242.976603
2017-10-05    243.126994
2017-10-15    273.699788
```

## Future Work

- Incorporate weather data (temperature, humditiy)
- Compare with other models (AutoRegressive Integrated Moving Average (ARIMA), Long Short-Term Memory (LSTM))
- Visualize feature importance and SHAP values
