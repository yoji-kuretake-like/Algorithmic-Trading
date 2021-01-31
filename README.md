# Algorithmic-Trading with R
## Goal for this notebook
<p>Predicting the Close price for the coming day, based on various key factors from historical days such as opening price(OP), closing price(CP), high price(HP), low price(LP), Relative Strength Index (RSI), and Exponential Moving Average (EMA), Moving Average Convergence Divergence (MACD). After the prediction, creating the trading strategies based on close price which was predicted and some technical indicators is required in order to make a profit. At the end, optimisation for the parameters of technical indicators should be done to get the highest profit. </p>

## Table of content
- Background to the problem
- An overview of the of data
- Details of the approach taken
- Presentation of and comments on the solutions achieved
- The performance of the model
- Comparison against other approaches
<p>This notebook is to perform Algorithmic trading including :</p>

### Close price prediction by Neural Networks
- Importing libraries and Loading data with quantmod
- Expranatoly data analysis (EDA)
- Technical indicator analysis
- Normalization of the data by min max scaler
- Create neural net model
- Evaluation
- Prediction
- Optimization of parameter

### Trading strategies
- Trading strategy based on exponential moving average
- Trading strategy based on MACD

### Parameters optimization
- Optimization of strategy based on exponential moving average
- Optimization of strategy based on MACD
