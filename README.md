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

   The Linear Regression model calculates the estimators of the regression coefficients or simply the predicted weights, denoted with 𝑏₀, 𝑏₁, …, 𝑏ᵣ. These estimators define the estimated regression function 𝑓(𝐱) = 𝑏₀ + 𝑏₁𝑥₁ + ⋯ + 𝑏ᵣ𝑥ᵣ which aims to discover the dependencies between the inputs and output sufficiently well. The estimated or predicted response, 𝑓(𝐱ᵢ), for each observation 𝑖 = 1, …, 𝑛, should be as close as possible to the corresponding actual response 𝑦ᵢ. The differences 𝑦ᵢ - 𝑓(𝐱ᵢ) for all observations 𝑖 = 1, …, 𝑛, are called the residuals. Regression is about determining the best predicted weights—that is, the weights corresponding to the smallest residuals. To get the best weights, you usually minimize the sum of squared residuals (SSR) for all observations 𝑖 = 1, …, 𝑛: SSR = Σᵢ(𝑦ᵢ - 𝑓(𝐱ᵢ))². This approach is called the method of ordinary least squares.

   The Autoregressive (AR) model predicts future values in a time series using its own past values as predictors. It assumes a linear relationship between the variable and its lagged values, aiming to capture patterns and trends for forecasting. Mathematically, the AR model is represented as x_t = c + ∑_{i=1}^{p} ϕ_i * x_{t-i} + ε_t, where x_t​ where ϕ_i​ are autoregressive coefficients.

4. **Simple/Exponential/Cross Moving Strategy Folder**
   - `simple_moving_strategy.py`: Contains the implementation of the simple moving average strategy.
   - `exponential_moving_strategy.py`: Contains the implementation of the exponential moving average strategy.
   - `cross_moving_strategy.py`: Contains the implementation of the crossover moving average strategy.

   The Simple, Exponential, and Cross Moving Average strategies are technical analysis tools used to identify trading signals based on moving averages of stock prices. These strategies are commonly used in algorithmic trading.

## Usage

Each folder contains Python scripts for the respective forecasting models or trading strategies. You can import and use these scripts in your own projects for stock forecasting and trading.

Feel free to explore the implementations and modify them according to your requirements.

