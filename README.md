# Machine Learning and Time Series Solutions for a Non-Linear Regression Problem (VAR, LSTM, Polynomial Regressions)
 
## 1. Exploratory Data Analysis
To understand what current situation is in data, to extract information of data and summarize the main characteristics of the data. 

* Descriptive analysis
* Visualization

## 2. Implementing of Polynomial Regression 
 
In this notebook, nonlinear modeling techniques were applied to predict continuous target in terms of regression.  

Applied several machine learning algortihms to predict number of hit. The best result is received by **LightGBM** algorithm which is one of the Gradient Boosting Trees. LightGBM has various tricks to make training more efficient and to improve performance and reduce the overfitting. It has different and more complicated tree split methodology which also makes it the better run. We also applied LightGBM for feature importance.

> **_<Note!>_**
> Due to dealing with real dataset, accuracies are not that much higher.

## 3. Multivariate Time Series LSTM Model & VAR Model 
In this code page, you will encounter the solutions via two different model approaches. First, apply multivariate LSTM for forecasting the click data. I use a quite base stateful LSTM model with 1 neuron fit for 20 epochs and 30 epochs. 

Also will see Vector Autoregression (VAR) that is a multivariate forecasting algorithm used when two or more time series influence each other.

> **_<Note!>_**
> Time series data preparation process has a few more steps compared to data mining process. 

> * **Cointegration Test :** The time series should influence each other. Check out whether time series are cointegrated, it means they have a long run, statistically significant relationship. <br/>
> * **Check for Stationarity and Make the Time Series Stationary :** For time series analysis, we need to be sure series are stationary.
> * **Decide the Order (P) of VAR model :** For our data decide on which lag is better to fit model. Choosed lowest AIC and other metrics.
> * **Transform the time series into a supervised learning problem for LSTM** 
> * **Check for Serial Correlation of Residuals :** Be sure residuals are randomly distributed which as known white noise.

Help you to reach listed sources that I have been received support. You can go to check out both of them which are quite good tutorials to first shot multivariate time series analysis.  

https://machinelearningmastery.com/use-timesteps-lstm-networks-time-series-forecasting/

https://www.machinelearningplus.com/time-series/vector-autoregression-examples-python/

<br/>

Good luck.
