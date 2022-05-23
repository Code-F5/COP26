# COP26
Data science project for predicting earth temperature using ARIMA,SARIMA and XG-BOOST algorithms.
The difference between ARIMA and SARIMA (SARIMAX) is about the seasonality of the dataset. if  data is seasonal, like it happen after a certain period of time then we will use SARIMA.
Time series is a series of data points measured at consistent time intervals such as yearly, daily, monthly, hourly and so on. It is time-dependent & the progress of time is an important aspect of the data set. One of the most common methods used in time series forecasting is known as the ARIMA model, which stands for Auto Regressive Integrated Moving Average. ARIMA is a model that can be fitted to time series data to predict future points in the series.
We can split the Arima term into three terms, AR, I, MA:
	• AR(p) stands for the autoregressive model, the p parameter is an integer that confirms how many lagged series are going to be used to forecast periods ahead.
	• I(d) is the differencing part, the d parameter tells how many differencing orders are going to be used to make the series stationary.
	• MA(q) stands for moving average model, the q is the number of lagged forecast error terms in the prediction equation. 
	SARIMA is seasonal ARIMA and it is used with time series with seasonality.
  
  There are a few steps to implement an ARIMA model:
 
	1.  Load the data & Import the necessary libraries :  math:Sqrt,
        sklearn.metrics:mean_squared_error,
        Pmdarima-->An ARIMA estimator.
        statsmodels.tsa.seasonal:seasonal_decompose->Seasonal decomposition using moving averages.
                                                        statsmodels.tsa.stattools:adfuller,
        matplotlib.pyplot,seaborn etc.
    2.  Data Preprocessing : While working with time series data in Python, it’s important to always ensure that dates are used as index values and are understood by Python as a true “date” object. We can do this by using pandas datestamp or to_datetime method.

    3.  Check for stationarity : Most time series models require the data to be stationary. A time series is said to be stationary if its statistical properties such as mean, variance & covariance remain constant over time. The formal ways to check for this are plotting the data and do a visual analysis and use a statistical test.
		* Visual: we can use the decomposition method which allows us to separately view seasonality (which could be daily, weekly, annual, etc), trend and random which is      the variability in the data set after removing the effects of the seasonality and trend.
[COP26_Final.pdf](https://github.com/Code-F5/COP26/files/8736203/COP26_Final.pdf)
