# Time_Series_Analysis_On_Electrical_Consumption

The project deals with electricity consumption in New York City between the years 2010 to 2022. The forecasting model is able to predict New York City’s Electricity Consumption by using Facebook’s Prophet model. Prophet is a procedure/model for forecasting time series data based on an additive model where non-linear trends are fit with yearly, weekly, and daily seasonality, on Daily, Monthly, and Yearly Mean electric consumption:

1) Monthly - The above daily data and average it out based on each month.
2) Yearly - The daily data and average it out based on each year.

The model is trained (on the respective dataset) to make future prediction on the Electric Consumption (EC) values from the last date of the dataset into X units of time into the future.
a) If the unit of time be day, then the EC is predicted for 100/200/365 days into the future.
b) If the unit of time be month, then the EC is predicted for 1/6/9 months into the future.
c) If the unit of time be year, then the EC is predicted for 1/10/20 years into the future.

The FBProphet model is also tuned using the following parameters:
a) Forecasting growth
b) Seasonality
c) Trend Changepoints

For each model, the predicted values are tabular printed and a line graph showing both historical data and the future is also depicted.

All models are evaluated by providing their respective MAE (Mean Absolute Error) and MAPE (Mean Absolute Percentage Error), as well as R^2 (use sklearn’s respective metrics).
 
Electric Consumption for each of the 5 Boroughs (independently) has also been done and the location with the highest is also depicted.
