# Stock Market Price Prediction

This project aims to predict stock market prices using the ARIMA (AutoRegressive Integrated Moving Average) time series forecasting model. 
By analyzing historical stock data, the ARIMA model can provide valuable insights and predictions for future price movements.

The project uses historical stock market data in CSV format. The data is stored in the data directory and should be structured with the following columns: 
Date, Open, High, Low, Close, Volume, and Adj Close

## ARIMA Model
The ARIMA model consists of three components:  

1. AutoRegressive (AR) Component: This component models the relationship between the current data point and its past values.
It uses lagged values of the time series data to predict future values. The "p" parameter in ARIMA represents the number of lagged values used in the model.
2. Integrated (I) Component: This component accounts for any trends or non-stationarity in the time series data by differencing the data points.
Differencing involves subtracting a time series from itself with a time lag, which helps make the data stationary (i.e., constant mean and variance).
The "d" parameter in ARIMA represents the number of differencing steps.
3. Moving Average (MA) Component: This component models the relationship between the current data point and the past forecast errors.
The "q" parameter in ARIMA represents the number of past forecast errors used in the model.
