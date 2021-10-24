# Demand-Forecasting

We have a Superstore dataset, having data from 2014 to 2017. Shows the product sold daily throughout US region. Need to forecast future demand of product for 2018 and 2019 i.e. upcoming 24 months.

Resampling done with resample() function so data changed with Monthly Frequency.

Applied Rolling statistics, that shows constant Mean and constant Standard Daviation. So it is a Stationary Dataset.

![image](https://user-images.githubusercontent.com/57244750/138581946-97f2ed83-2a5b-4806-96bf-f51ae70d5e1d.png)



As here in the dataset seasonality was included so SARIMAX was used. So accordingly to Test data, prediction is done as below.

![image](https://user-images.githubusercontent.com/57244750/138581994-758b4bb8-9d96-468a-ac19-e46b12d002ae.png)


After that considering the Final goal of the project, we need to predict demand for upcoming two years. i.e. year 2018 and 2019. 
predict function applied and below as the forecast:

![image](https://user-images.githubusercontent.com/57244750/138582066-50b6b5b9-700c-40f3-b749-7bcaf00e0b88.png)


**Concepts to be learnt:**

Stationarity Check, if dataset is stationary:

**Dickey-Fuller Test**

A Dickey-Fuller test is a unit root test that tests the null hypothesis that α=1 in the following model equation. alpha is the coefficient of the first lag on Y.

Null Hypothesis (H0): alpha=1

where,

y(t-1) = lag 1 of time series.
delta Y(t-1) = first difference of the series at time (t-1).
Fundamentally, it has a similar null hypothesis as the unit root test. That is, the coefficient of Y(t-1) is 1, implying the presence of a unit root. If not rejected, the series is taken to be non-stationary.

**SARIMAX**
SARIMAX(Seasonal Auto-Regressive Integrated Moving Average with eXogenous factors) is an updated version of the ARIMA model. ARIMA includes an autoregressive integrated moving average, while SARIMAX includes seasonal effects and eXogenous factors with the autoregressive and moving average component in the model. Therefore, we can say SARIMAX is a seasonal equivalent model like SARIMA and Auto ARIMA.

![image](https://user-images.githubusercontent.com/57244750/138582504-34c073f8-b03f-40c1-8765-5950c79b70eb.png)

![image](https://user-images.githubusercontent.com/57244750/138582514-ee4a7415-d772-47f1-b63c-da13f2340f96.png)




