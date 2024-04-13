# Stock Forecasting Project

This repository contains implementations of stock forecasting models and strategies in Python. The project is organized into two main folders:

1. **Linear/Auto Regression Model Folder**
   - `LR_AR.py`: Contains the implementation of the linear and auto regression forecasting model with computed coefficient of determination of R².

   The Linear Regression (LR) model estimates regression coefficients (𝑏₀, 𝑏₁, …, 𝑏ᵣ) to create the function 𝑓(𝐱) = 𝑏₀ + 𝑏₁𝑥₁ + ⋯ + 𝑏ᵣ𝑥ᵣ, which reveals dependencies between inputs and output. It aims to make the predicted response 𝑓(𝐱ᵢ) as close as         possible to the actual response 𝑦ᵢ for each observation 𝑖 = 1, …, 𝑛. The differences 𝑦ᵢ - 𝑓(𝐱ᵢ) across all observations 𝑖 = 1, …, 𝑛 are residuals. Regression finds the best predicted weights by minimizing the sum of squared residuals (SSR) for all       observations 𝑖 = 1, …, 𝑛: SSR = Σᵢ(𝑦ᵢ - 𝑓(𝐱ᵢ))² using the ordinary least squares method.

   The Autoregressive (AR) model predicts future values using past values, assuming a linear relationship. It captures patterns and trends in time series data. The AR model is mathematically represented as xₜ = c + ∑ from i=1 to p (ϕᵢ * xₜ₋ᵢ) + εₜ
   where xₜ and ϕᵢ are autoregressive coefficients.

2. **Simple/Exponential/Cross Moving Strategy Folder**
   - `SMA_Signals.ipynb`: Contains the implementation of the simple moving average strategy by utilizing the .rolling function to create rolling average of varying window lengths. The code then attaches buy/sell indicators and plots the result.
   - `EMA_Signals.ipynb`: Contains the implementation of the exponential moving average strategy by utilizing the .ewm function to compute the exponentially weighted moving average with a varying number of data points. The code then attaches buy/sell                            indicators and plots the result.
   - `MA_CrossStrategy.ipynb`: Contains the implementation of the crossover moving average strategy which allows the user to specify whether they want to compute the SMA or the EMA for multiple tickers and also returns the buy/sell indicator table.

   The Simple, Exponential, and Cross Moving Average strategies are technical analysis tools used to identify trading signals based on moving averages of stock prices.

