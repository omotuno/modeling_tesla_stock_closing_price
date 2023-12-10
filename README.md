# Tesla Stock Price Modeling

This time series analysis project models and forecasts the closing price of Tesla stock. Daily closing prices from 2010-2020 are analyzed to determine an appropriate ARIMA model.

### The analysis follows these steps:

-- Loading and plotting the Tesla closing price time series data
<img width="864" alt="Screenshot 2023-12-10 at 4 52 02 PM" src="https://github.com/omotuno/modeling_tesla_stock_closing_price/assets/65866718/d80a00ff-7ab6-4483-928f-23126aa8b55a">

-- Applying a log transformation to stabilize variance

-- Taking first differences to make the series stationary

-- Examining ACF and PACF plots to identify potential ARIMA models

-- Taking second differences due to lack of clear model from initial plots

-- Concluding the differenced series resembles white noise and lacks structure for modeling

-- The transformations were unsuccessful in revealing autocorrelation structure that could be modeled with an ARIMA model. The data exhibits behavior close to a random walk. Other techniques like machine learning may be better suited for generating forecasts.


