# Time-Series-Store-Sales-Forecasting
Time series forecasting involves predicting future values based on past data trends for example in predicting store sales. Examples of models: Error, Trend Seasonality (ETS), Autoregressive Integrated Moving Average (ARIMA) and Seasonal ARIMA(SARIMA). ARIMA adopts better to non-seasonal data while ETS is the model of choice for data that shows robust and consistent seasonal patterns ( Gao, 2025).
This was research on predictive analysis carried out on Time Series as a Kaggle.com Competition. The assignemnt was in forecasting a store’s sales using Error, Trend, Season (ETS), and Autoregressive Integrated Moving Average (ARIMA)

Results for the ETS Store Sales Forecasting Model(Time Series) 
RMSLE Score (0.0981). This indicates the ETS model has an average logarithmic error of about 9.81%. In practical terms, this means that the forecasts are typically within ±10% of actual values. For retail sales forecasting, an RMSLE < 0.1 is generally considered good performance.
Residuals: 
They appear distributed around zero with no clear pattern. There is no visible time dependent structure , meaning there is no heteroskedasticity. A few outliers are present but there is no bias . The histogram shape suggests that errors are normally distributed.. There is some larger errors as indicated by tails but no severe skewness

SARIMA Store Sales Forecasting Model (Time Series)
RMSLE Score (0.1171):
The model achieves a Root Mean Squared Logarithmic Error of 0.1171.
This translates to approximately ±11.7% average error in the forecasts
For retail sales forecasting, RMSLE < 0.1 is typically considered excellent, so the model is performing well but has room for improvement!
Forecast Visualization:
The forecast (red line) closely tracks actual sales (blue line) which is optimal.
Confidence bands remain reasonably tight, indicating stable predictions.
The model appears to capture both the trend and weekly seasonality patterns.

According to Gao (2025) ARIMA and ETS are prominent forecasting methods and should have their efficacy evaluated against seasonal data sets. He argues that seasonal patterns are more predictive of the future and  ARIMA models are popular in predicting financial outcomes in time series because this is data that lacks seasonal patterns. Furthermore,  the author  suggests that ETS surpasses ARIMA in analyzing data that contains seasonal trends since ARIMA fails to account for these patterns. It would seem that Gao (2025), is correct and his claims mirror my research in the head to head of ARIMA versus ETS. ETS had a Root Mean Standard Logarithmic Error  (RMSLE) of 0.098 while for the same store dataset ARIMA had an RMSLE of 0.1171. It is not to downplay ARIMA’s RMSLE but ETS had  a better metric below the ideal < 0.1 for forecasting retail store sales. Due to the ETS ability to capture trend and seasonality which are present in the data set.

References:

Gao, Yijun. (2025). A Comparative study of ARIMA and ETS models for time series forecasting. Advances 	in Economics, Management and Political Sciences, 149, 196-201. https://doi.org/10.54254/2754-1169/2024.19252.
