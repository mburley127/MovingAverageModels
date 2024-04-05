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

   The Linear and Auto Regression models use historical data to identify trends and patterns for making future predictions. These models are based on statistical analysis and regression techniques.

3. **Simple/Exponential/Cross Moving Strategy Folder**
   - `simple_moving_strategy.py`: Contains the implementation of the simple moving average strategy.
   - `exponential_moving_strategy.py`: Contains the implementation of the exponential moving average strategy.
   - `cross_moving_strategy.py`: Contains the implementation of the crossover moving average strategy.

   The Simple, Exponential, and Cross Moving Average strategies are technical analysis tools used to identify trading signals based on moving averages of stock prices. These strategies are commonly used in algorithmic trading.

## Usage

Each folder contains Python scripts for the respective forecasting models or trading strategies. You can import and use these scripts in your own projects for stock forecasting and trading.

Feel free to explore the implementations and modify them according to your requirements.

