# Apple Stock Analysis using R

## Overview
This project aims to analyze the historical stock prices of Apple Inc. (AAPL) using R. The analysis includes data visualization and statistical metrics to uncover trends and insights that can assist in investment decisions.


## Installation
To get started, clone this repository to your local machine and install the required R packages:


##Data
The dataset used in this analysis includes historical stock price data for Apple Inc. (AAPL) from Yahoo Finance. The data includes the following columns:

Date
Open
High
Low
Close
Volume
Adjusted Close


Key Observations:

1.  ARIMA Model:

    coefficient=0.081, with std. error of 0.0392=\> Showing **slight Upward Trend**

    MAE=1.93, which indicates on average , ARIMA model is off by 1.94 units in predicting stock price

    AIC =10185.24, which is lower so suitable for model.

2.  Prophet model:

    MAE = 10.065, which is very higher than ARIMA model's MAE, So prophet model is performing worse.

Analysis:

1.  ARIMA(0,1,0) with drift: slight upward trend

    suitable model for financial data

    low MAE and RMSE which is good with minimal error

2.  Prophet model:it is struggling with this data because emphasize on trend and seasonality, which is showing difficulty in stock price data.

Result: ARIMA wins: It's more accurate for this data set than prophet. it can also handle easily random fluctuations.
