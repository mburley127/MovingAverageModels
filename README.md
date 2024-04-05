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

   The Linear Regression model estimates regression coefficients (𝑏₀, 𝑏₁, …, 𝑏ᵣ) to create the function 𝑓(𝐱) = 𝑏₀ + 𝑏₁𝑥₁ + ⋯ + 𝑏ᵣ𝑥ᵣ, which reveals dependencies between inputs and output. It aims to make the predicted response 𝑓(𝐱ᵢ) as close as possible     to the actual response 𝑦ᵢ for each observation 𝑖 = 1, …, 𝑛. The differences 𝑦ᵢ - 𝑓(𝐱ᵢ) across all observations 𝑖 = 1, …, 𝑛 are residuals. Regression finds the best predicted weights by minimizing the sum of squared residuals (SSR) for all                observations 𝑖 = 1, …, 𝑛: SSR = Σᵢ(𝑦ᵢ - 𝑓(𝐱ᵢ))² using the ordinary least squares method.

   The Autoregressive (AR) model predicts future values using past values, assuming a linear relationship. It captures patterns and trends in time series data. The AR model is mathematically represented as x_t = c + ∑_{i=1}^{p} ϕ_i * x_{t-i} + ε_t,       where x_t​ and ϕ_i​ are autoregressive coefficients.

3. **Simple/Exponential/Cross Moving Strategy Folder**
   - `SMA_Signals.py`: Contains the implementation of the simple moving average strategy.
   - `EMA_Signals.py`: Contains the implementation of the exponential moving average strategy.
   - `MA_CrossStrategy.py`: Contains the implementation of the crossover moving average strategy.

   The Simple, Exponential, and Cross Moving Average strategies are technical analysis tools used to identify trading signals based on moving averages of stock prices. These strategies are commonly used in algorithmic trading.

