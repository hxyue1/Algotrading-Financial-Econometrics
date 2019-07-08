# Algotrading-Financial-Econometrics

An ongoing financial econometrics project working with Vanguard ETF prices in hopes of building an algorithmic trading model to read in new data, adjust daily allocations based on forecasted returns and volatilities and make trades through an online broker.

## What's been done so far

### Modelling returns
- Exploration of data using ACFs and histograms
- Estimation of AR, ARMA and ARIMA models (note that in most cases estimation of ARMA and ARIMA models fails so AR models are evaluated instead)
- Evaluation of forecasting models using rolling one-step ahead forecasts to determine whether or not the EMH holds and how much better the model will perform than assuming a constant returns model

### Modelling volatility 
- Estimation of GJR-GARCH models with various distributional assumptions
- Normality is in strong violation in all circustances due to negative skewness and high kurtosis
- Student's-t, skewed Student's-t and the generalised hyperbolic distribution are entertained as potential distributions
- Standardised residuals are evaluated using QQplots to check distributional assumptions

## What's to be done in the future
- Evaluation of volatility forecasting models using demeaned squared returns (noisy estimator) or the Parkinson's estimator
- Calculation of Value at Risk using distributional assumptions and Extreme Value approach
- Multivariate returns and volatility models
- Evalation of forecasting capacity of multivariate models
- Portfolio selection with the objective of maximising daily sharpe ratio, and evaluation of such an algorithm
- Creation of alternative algorithms and performance evaluation of those algorithms
- End-to-end project with data automatically scraped and updated every day and portfolio alocation sent to broker
