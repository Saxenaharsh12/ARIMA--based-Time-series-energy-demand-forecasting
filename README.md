# ARIMA--based-Time-series-energy-demand-forecasting

# USE CASE/ OBJECTIVE - Company wants to predict electricity demand accurately to optimize power generation and distribution. We predict future energy demand using greater precision which helps energy supplier to better plan and manage their resources.

# APPROACH- 
Time series data from past years,including historical demand,weather data, holidays was collected. ARIMA model is used to capture seasonality and trends.
Deep AR is applied for probabilistic forcasting with prediction intervals.

# OUTCOME- Accurate forecasts enabled utility company to optimize power generation,reduce operational costs and prevent energy shortages during peak-demand periods.


# Introduction- Time Series.

# WHAT IS TIME SERIES ANALAYSIS?

Time Series: Set of observations taken at a specified time usually at equal intervals. It is used to predict future values based on previous observed values.

Considering a graph, when x is time & if the dependent variable depends on time parameter then it’s time series analysis.

# COMPONENTS OF TS ANALYSIS:

Trend

Seasonality

Irregularity

Cyclic

# STATIONARITY?

TS data can be stationary by removing:

Trend - Varying over time
Seasonality - Variations at specific time
How?

Constant mean - Average
Constant variance - Distance from mean
Auto covariance that does not depend on time
HOW TO TEST STATIONARITY?

Rolling Statistics: Visual technique

# Augmented Dickey Fuller Test: �Here the null hypothesis is that the TS is non-stationary.�If ‘Test Statistics’ < ‘Critical Value’(0.05), then we can reject the hypothesis & conclude that TS is stationary.

# ARIMA:

Auto Regression: Auto Regressive lags, If there’s a correlation between t & t-5, then that’s an autoregressive model If p is 5, then predictors of x(t) = x(t-1)….x(t-5)

Moving Average: Lagged forecast errors in prediction. If q is 2, predictors of x(t) will be e(t-1)..e(t-2) e(i) is the difference between moving average of ith instance & actual value

ACF: Auto Correlation function, it’s the measure of correlation between TS and the lagged value of itself. PACF: Partial Auto Correlation function, it’s the correlation of TS with a lagged value of itself but after removing variation.

# LSTM (Long Short Term Memory)

Recurrent Neural Network:

Vector to Sequence – I/P (Image)  Describes an image Example: Image Captioning Sequence to Vector – I/P(Product Reviews)  O/P is in form of a vector [0.9 0.1] of positive: negative Example: Sentiment Analysis Sequence to Sequence – I/P(Sequence)  O/P(Sequence) It’s based on Encoder-Decoder Architecture Example: Translation

TS data is actually sequences.
When dealing with weather data  Precipitation, Rain, Temperature etc.
Where some of the features can be relevant for forecasting, weather entirely is treated as a vector & is i/p to the neural network.
TS can be modelled as a sequence to sequence problem


# PROPHET:

When fbProphet shines?

Hourly, Weekly, Daily observations with at least a few months of history.
Strong multiple “human-scale” seasonality's
Holidays that occur at irregular intervals
Reasonable number of missing observations



