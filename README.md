# Master-s-Project

ARIMA- 'AutoRegressive Integrated Moving Average'

The general process for ARIMA models is the following:
-Visualize the Time Series Data
-Make the time series data stationary
-Plot the Correlation and AutoCorrelation Charts. It tells about
    the lag values incase of AutoRegressive and Moving Average.
-Construct the ARIMA Model or Seasonal ARIMA based on the data
-Use the model to make predictions

To find if the data is stationary or not we perform Dickey-Fuller test.
We use adfuller function to perform the test and it gives us 4 different values:
ADF Test Statistic
p-value
Lags Used
Number of Observations Used
What we require is p-value. We can consider that if p-value < 0.05 we reject null hypothesis or we fail to reject null hypothesis.
H0= It is not Stationary
H1= It is Stationary

Identification of an AR model is often best done with the PACF.
For an AR model, the theoretical PACF “shuts off” past the order of the model. The phrase “shuts off” means that in theory the partial autocorrelations are equal to 0 beyond that point. Put another way, the number of non-zero partial autocorrelations gives the order of the AR model. By the “order of the model” we mean the most extreme lag of x that is used as a predictor.

Identification of an MA model is often best done with the ACF rather than the PACF.
For an MA model, the theoretical PACF does not shut off, but instead tapers toward 0 in some manner. A clearer pattern for an MA model is in the ACF. The ACF will have non-zero autocorrelations only at lags involved in the model.


Benifits:
The main advantage of ARIMA forecasting is that it requires data on the time series in question only. First, this feature is advantageous if one is forecasting a large number of time series. 
Second, this avoids a problem that occurs sometimes with multivariate models. For example, consider a model including wages, prices and money. It is possible that a consistent money series is only available for a shorter period of time than the other two series, restricting the time period over which the model can be estimated.


Challenges:
ARIMA models are essentially ‘backward looking’. As such, they are generally poor at predicting turning points, unless the turning point represents a return to a long-run equilibrium.


I am working on Fast Fourier Transform to check how the dataset would look for forecasting.

