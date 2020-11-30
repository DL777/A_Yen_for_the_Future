# A_Yen_for_the_Future

# Background
The financial departments of large companies often have to make foreign currency transactions when doing international business, while hedge funds are also interested in anything that will provide an edge in predicting currency movements. Hence, both are always eager to gain a better understanding of the future direction and risk of various currencies.

In this assignment, you will test the many time series tools that you have learned in order to predict future movements in the value of the Canadian dollar versus the Japanese yen.

You will gain proficiency in the following tasks:

1. Time series forecasting
2. Linear regression modelling



# Files
Time-Series Starter Notebook

Linear Regression Starter Notebook

CAD/JPY Data CSV File

# The Summary of the Analysis

In this analysis, the CAD/JPY exchange rate was modelled using the *time-series* and *linear regression* techniques.

In the **Time Series** part, the CADJPY exchange rate time series were broken down into the *Trend* and *Noise* parts using the Hodrick-Prescott Filter. 
The CADJPY exchange rate daily returns were then modelled as ARMA (2,1) process which was found to have only one statistically significant auto-regressive lag.

The CADJPY exchange rate was also modelled as ARIMA (5,1,1) process. None of the auto-regressive lags in this model were found to be statistically significant.

Following this, the volatility of the CADJPY exchange rate was modelled as GARCH (2.1) process.

In the **Linear Regression** part of the analysis, the CADJPY exchange rate daily returns were regressed on their one-period lagged values. The model produced a poor fit with R^2 of 0. Also, quite unexpectedly, the model had a better the out-of-sample performance then the in-sample performance.

# Conlclusion

While the results produced by the Time Series models are promising, a further model optimization is required before they can be implemented for trading. 