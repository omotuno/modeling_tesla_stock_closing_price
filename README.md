# Tesla Stock Price Modeling

This time series analysis project models and forecasts the closing price of Tesla stock. Daily closing prices from 2010-2020 are analyzed to determine an appropriate ARIMA model.

### The analysis follows these steps:

-- Loading and plotting the Tesla closing price time series data
<img width="864" alt="Screenshot 2023-12-10 at 4 52 02 PM" src="https://github.com/omotuno/modeling_tesla_stock_closing_price/assets/65866718/d80a00ff-7ab6-4483-928f-23126aa8b55a">

-- Applying a log transformation to stabilize variance
<img width="846" alt="Screenshot 2023-12-10 at 4 53 27 PM" src="https://github.com/omotuno/modeling_tesla_stock_closing_price/assets/65866718/2dc2a7d2-7539-4301-95bb-b4bdec014810">
<img width="810" alt="Screenshot 2023-12-10 at 4 53 42 PM" src="https://github.com/omotuno/modeling_tesla_stock_closing_price/assets/65866718/c38ea310-123d-42a4-a219-c50afc338fa6">

-- Taking first differences to make the series stationary
<img width="842" alt="Screenshot 2023-12-10 at 4 53 54 PM" src="https://github.com/omotuno/modeling_tesla_stock_closing_price/assets/65866718/e1952cfa-187a-46c3-a1ca-a6b9fb3851a8">

-- Examining ACF and PACF plots to identify potential ARIMA models
<img width="856" alt="Screenshot 2023-12-10 at 4 54 13 PM" src="https://github.com/omotuno/modeling_tesla_stock_closing_price/assets/65866718/f9929ff8-21f2-4456-939c-64ed21229b72">

-- Taking second differences due to lack of clear model from initial plots
<img width="859" alt="Screenshot 2023-12-10 at 4 54 34 PM" src="https://github.com/omotuno/modeling_tesla_stock_closing_price/assets/65866718/7a0792b5-9048-4d8c-897f-b54e5b801b89">

-- Concluding the differenced series resembles white noise and lacks structure for modeling

-- The transformations were unsuccessful in revealing autocorrelation structure that could be modeled with an ARIMA model. The data exhibits behavior close to a random walk. Other techniques like machine learning may be better suited for generating forecasts.


