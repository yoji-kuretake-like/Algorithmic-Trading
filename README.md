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

## Background to the problem

<p>In this report we will explore the use techniques for automatically formulating trading rules using Artificial Intelligence models. One powerful instrument is the Neural Network. Artificial Neural networks are inspired by brain structure; they are composed of many neurons. Depending on its inputs, a particular set of neurons are activated and propagate a transformed signal, through application of a number of a non-linear functions. A Multilayer perceptron (MLP) is an ANN that consists of layers of neurons (an input, multiple hidden and an output layers). All neurons in a layer are fully connected to all neurons in the next layer. Therefore, the information always moves forward from inputs to outputs nodes. The Universal Approximation Theorem says a MLP with a single hidden layer and enough neurons can approximate any function either linear or nonlinear .</p>

<p>Using the power of ANNs we are able to model complex structures that historical financial data follows.

We wil use the neural network for prediction of future stock values with the use of two trading strategies based on EMA and MACD to make a profit in the stock trading. In addition, we will optimize the parameters of EMA and MACD to increase the profit more than default parameters.</p>

<p>The following are some research papers we evaluated and inspired our work greatly as this is a very promiment tool for leading investment banks/funds.</p>

- Arévalo, Andrés & Nino, Jaime & Hernandez, German & Sandoval, Javier & León, Diego & Aragón, Arbey. (2017). Algorithmic Trading Using Deep Neural Networks on High Frequency Data. 144-155. 10.1007/978-3-319-66963-2_14.

- Alain P. Chaboud Benjamin Chiquoine Erik Hjalmarsson Clara Vega.(2014) Rise of the Machines: Algorithmic Trading in the Foreign Exchange Market.
