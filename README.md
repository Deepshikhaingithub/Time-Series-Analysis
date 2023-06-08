# Time-Series-Analysis
Time-Series-Analysis on HCLTech stock price

This project aims to analyze the stock prices of the company HCLTECH from 2000 to 2020. The dataset used for this analysis contains detailed information about the stock prices, including the date, symbol, series, opening price, closing price, volume, and other relevant variables.

**Dataset Description**

The dataset consists of the following columns:

Date: Represents the date of the recorded data.
Symbol: Represents the symbol or ticker of the company associated with the data (HCLTECH in this case).
Series: Represents the type of series or segment the data belongs to (EQ for equity).
Prev Close: Closing price of the stock from the previous trading day.
Open: Opening price of the stock for the given trading day.
High: Highest price reached by the stock during the trading day.
Low: Lowest price reached by the stock during the trading day.
Last: Last traded price of the stock for the trading day.
Close: Closing price of the stock for the trading day.
VWAP: Volume Weighted Average Price, calculated by dividing the total value of all trades by the total trading volume for the day.
Volume: Total number of shares or contracts traded during the day.
Turnover: Total value of the trades executed during the day.
Trades: Number of trades that took place during the trading day.
Deliverable Volume: Volume of shares or contracts that were physically delivered or settled.
%Deliverble: Percentage of the total traded volume that corresponds to the deliverable volume.

**Analysis Performed**

The analysis focuses on the stock prices of HCLTECH for the year 2013. The following steps were performed:

--Data Cleaning: The dataset was cleaned to ensure consistency and remove any inconsistencies or errors.

--Treating Missing Values: Missing values in the dataset were handled using appropriate techniques.

--Visualizing Actual Time Series: The actual time series data was visualized to understand the underlying patterns and trends.

--Checking Stationarity: Rolling statistics were used to determine the stationarity of the time series. The series was found to be non-stationary.

--Log Transformation: To make the series stationary, a log transformation was applied to the data.

--Differencing: Differencing was performed on the log-transformed data to achieve stationarity.

--Visualizing Stationarity: Rolling statistics were again used to check the stationarity of the differenced data.

--Building ARIMA Model: An ARIMA (AutoRegressive Integrated Moving Average) model was constructed using the stationary time series data.

--Order Selection: Autocorrelation Function (ACF) and Partial Autocorrelation Function (PACF) were used to determine the appropriate order of Auto Regression (AR) and Moving Average (MA) for the ARIMA model.

--Model Training: The ARIMA model was trained using the selected order.

--Model Evaluation: The fitted values of the model were plotted alongside the differenced data to assess the model's performance.

--Inverse Transformations: Since multiple transformations were applied, the original time series was retrieved using cumulative sum and transformed back using exponential.

--ARIMA Predictions: The ARIMA model was used to make predictions on the original time series data.

--Model Performance: The Root Mean Squared Error (RMSE) was calculated to evaluate the performance of the ARIMA model.

This project provides insights into the stock price patterns of HCLTECH and demonstrates the application of time series
