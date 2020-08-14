# MachineLearning-Time_Series-Project

## Background

The financial departments of large companies often have to make foreign currency transactions when doing international business, while hedge funds are also interested in anything that will provide an edge in predicting currency movements. Hence, both are always eager to gain a better understanding of the future direction and risk of various currencies. 

In this project, many time series tools were used in order to predict future movements in the value of the Canadian dollar versus the Japanese yen.

The following were used in the following tasks:

1. Time series forecasting
2. Linear regression modelling

Language Used: Python with Pandas used for data cleaning


- - -

### Files

[Time-Series Starter Notebook](Starter_Code/time_series_analysis.ipynb)

[Linear Regression Starter Notebook](Starter_Code/regression_analysis.ipynb)

[CAD/JPY Data CSV File](Starter_Code/cad_jpy.csv)

- - -

### Steps:

#### Time-Series Forecasting

In this notebook (time_series_analysis.ipynb), the historical CAD-JPY exchange rate data was loaded and time series analysis and modelling was applied to determine if there is any predictable behaviour.

The following steps were completed to create a machine learning **Model** which was then **Fitted** and made useful to **Predict** the values:

1. Decomposition using a Hodrick-Prescott filter (decompose the settle price into trend and noise).
2. Forecasting returns using an ARMA model.
3. Forecasting the exchange rate price using an ARIMA model.
4. Forecasting volatility with GARCH.

The results of the time series analysis and modelling were used to answer the following questions:

1. Based on the time series analysis, would you buy the yen now?
2. Is the risk of the yen expected to increase or decrease?
3. Based on the model evaluation, would an investor feel confident in using these models for trading?

#### Linear Regression Forecasting

In this notebook (linear_regression.ipynb), a Scikit-Learn linear regression model was built to predict CAD/JPY returns with *lagged* CAD/JPY futures returns and categorical calendar seasonal effects (e.g., day-of-week or week-of-year seasonal effects).

The following tasks were accomplished in the outlined order:

1. Data preparation (created returns and lagged returns, and splitted the data into training and testing data)
2. Fit a linear regression model.
3. Make predictions using the testing data.
4. Out-of-sample performance.
5. In-sample performance.

Using the results of the linear regression analysis and modelling the following question was answered:

* Does this model perform better or worse on out-of-sample data compared to in-sample data?

- - -

### Considerations

* Out-of-sample data is data that the model hasn't seen before (testing data).
* In-sample data is data that the model was trained on (training data).

- - -