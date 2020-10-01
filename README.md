# Yen Futures return Forecasting using Time Series Analysis

![Yen Photo](Resources/Japanese_Market.png)

## Background

The financial departments of large companies often deal with foreign currency transactions while doing international business. As a result, they are always looking for anything that can help them better understand the future direction and risk of various currencies. Hedge funds, too, are keenly interested in anything that will give them a consistent edge in predicting currency movements.

### Time Series Analysis

In this Notebook, we will leverage time-series analysis tools in order to predict future movements in the value of the Japanese yen versus the U.S. dollar.

Using the historical Dollar-Yen exchange rate futures data (yen.csv - in resources folder) we will apply time series analysis and modeling to determine whether there is any predictable behavior.

Below steps have been incorporated in the time-series analyis notebook :

1. Decomposition using a Hodrick-Prescott Filter (Decompose the Settle price into trend and noise).
2. we will use ACF and PACF to identify signifiant lags that can be used in ARMA and ARIMA models
3. Forecasting Returns using an ARMA Model.
4. Forecasting the Settle Price using an ARIMA Model.
5. Forecasting Volatility with GARCH.

Using the results of the time series analysis and modeling we shall answer the following questions:

1. Based on your time series analysis, would you buy the yen now?
2. Is the risk of the yen expected to increase or decrease?
3. Based on the model evaluation, would you feel confident in using these models for trading?


### Linear Regression Forecasting

In this notebook, you will build a Scikit-Learn linear regression model to predict Yen futures ("settle") returns with *lagged* Yen futures returns.

The steps outlined below have been incroprated in the regression_analysis notebook to create and evaluate the model:

1. Data Preparation (Creating Returns and Lagged Returns and splitting the data into training and testing data)
2. Fitting a Linear Regression Model.
3. Making predictions using the testing data.
4. Out-of-sample performance.
5. In-sample performance.

Using the results of the linear regression analysis and modeling the following question will be addressed:

* Does linear regression analysis model perform better or worse on out-of-sample data compared to in-sample data?