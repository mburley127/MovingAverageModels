# Stock Forecasting Project

This repository contains implementations of stock forecasting models and strategies in Python. The project is organized into three main folders:

2. **Simple/Exponential/Cross Moving Strategy Folder**
   - `SMA_Signals.ipynb`: Contains the implementation of the simple moving average strategy by utilizing the .rolling function to create rolling average of varying window lengths. The code then attaches buy/sell indicators and plots the result.
   - `EMA_Signals.ipynb`: Contains the implementation of the exponential moving average strategy by utilizing the .ewm function to compute the exponentially weighted moving average with a varying number of data points. The code then attaches buy/sell                            indicators and plots the result.
   - `MA_CrossStrategy.ipynb`: Contains the implementation of the crossover moving average strategy which allows the user to specify whether they want to compute the SMA or the EMA for multiple tickers and also returns the buy/sell indicator table.

   The Simple, Exponential, and Cross Moving Average strategies are technical analysis tools used to identify trading signals based on moving averages of stock prices.

