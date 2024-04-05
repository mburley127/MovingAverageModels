# Stock Forecasting Project

This repository contains implementations of stock forecasting models and strategies in Python. The project is organized into three main folders:

1. **Monte Carlo Forecast Folder**
   - `MC_Main.py`: Contains the implementation of the Monte Carlo forecasting model.
   - `MC_Functions.ipynb`: Contains the functions required to implement the Monte Carlo forecasting model.
   - `Price_Paths.ipynb`: Contains the introductory project to first calculate the daily price changes using the geometric Brownian motion formula, then compute the price at each time step based on the previous price and the corresponding daily return

   The Monte Carlo forecast uses random sampling techniques to simulate various future scenarios based on historical data. It is useful for generating probabilistic forecasts.

2. **Linear/Auto Regression Model Folder**
   - `linear_regression_model.py`: Contains the implementation of the linear regression forecasting model.
   - `auto_regression_model.py`: Contains the implementation of the auto regression forecasting model.

The Linear Regression (LR) model calculates the estimators of the regression coefficients or predicted weights, denoted as b0,b1,...,brb0​,b1​,...,br​. These estimators define the estimated regression function f(x)=b0+b1x1+...+brxrf(x)=b0​+b1​x1​+...+br​xr​ aiming to discover dependencies between inputs and output. The estimated or predicted response f(xi)f(xi​) for each observation i=1,...,ni=1,...,n should be as close as possible to the actual response yiyi​. The differences yi−f(xi)yi​−f(xi​) for all observations i=1,...,ni=1,...,n are called residuals. Regression minimizes the sum of squared residuals (SSR) for all observations i=1,...,ni=1,...,n: SSR = ∑i(yi−f(xi))2∑i​(yi​−f(xi​))2, using the method of ordinary least squares.

The Autoregressive (AR) model predicts future values in a time series using its own past values as predictors. It assumes a linear relationship between the variable and its lagged values, capturing patterns and trends for forecasting. Mathematically, the AR model is represented as xt=c+∑i=1pϕixt−i+ϵtxt​=c+∑i=1p​ϕi​xt−i​+ϵt​, where xtxt​ represents the value at time tt, ϕiϕi​ are autoregressive coefficients, and pp is the order of autoregression.

4. **Simple/Exponential/Cross Moving Strategy Folder**
   - `simple_moving_strategy.py`: Contains the implementation of the simple moving average strategy.
   - `exponential_moving_strategy.py`: Contains the implementation of the exponential moving average strategy.
   - `cross_moving_strategy.py`: Contains the implementation of the crossover moving average strategy.

   The Simple, Exponential, and Cross Moving Average strategies are technical analysis tools used to identify trading signals based on moving averages of stock prices. These strategies are commonly used in algorithmic trading.

## Usage

Each folder contains Python scripts for the respective forecasting models or trading strategies. You can import and use these scripts in your own projects for stock forecasting and trading.

Feel free to explore the implementations and modify them according to your requirements.

