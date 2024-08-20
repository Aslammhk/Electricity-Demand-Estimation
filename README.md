# Electricity-Demand-Estimation
Electricity Demand Estimation for Leading Electricity Distributor.

# Solution Data pipelines.

Import packages that are crucial, then read the respective data files.

Data Preprocessing - a. Create Year_Month column and set it as index. Also create Year, and Month as separate columns for future reference. b. Visualize the data in graphical format for better understanding of the data. c. Create pivot table with index = Year and Columns = Month, Values = Electricity_Consumption d. Visualize the pivot table data into axes subplot for clear separation.

Decomposition of data - a. To decompose the data we utilize the seasonal decompose package. b. Seasonal decompose package contains two types - additive and multiplicative. c. Additive decomposition is applied to understand the time series data thoroughly. d. Additive decompose is applied to the dataset because when the data is related to time series then level, trend, seasonality, and noise are computed.

Perform AutoCorrelation and Partial Autocorrelation tests to indicate a model would be appropriate for the time series because the ACF cuts after one lag while the PACF shows a slowly decreasing trend.

Perform a statistical significance test to check whether time series data is stationary or not. The augmented Dickey-Fuller test is used to determine the solution.

Apply Exponential Smoothing to focus on trend and seasonal components. This data is then used to present or to make forecasts.

Apply train test split to overcome the problem of overfitting.

Perform seasonal ARIMA test for explicit support to univariate time series data with the seasonal components.

Now model can be used to make a forecast. Found the model train error is too minimal hence the model provides higher accuracy.

To check the accuracy, we employ different metrics such as MAPE, RMSE, and RMSPE.

To forecast the demand for electricity and to visualize the result of the same new line graph is generated along with diagnostics().
