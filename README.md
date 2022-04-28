# Basket pricing using Neural Networks

### Challange:

The client wants to explore novel methodologies for accelerating the pricing of exotic derivatives. 

### Goal: 
ANN approach to reduce the computing time of pricing
financial options

We test the ANN approach on
three different solvers, including the closed-form solution for the Black-Scholes equation

The goal is to build and train a neural network model for [pricing](https://www.investopedia.com/articles/optioninvestor/07/options_beat_market.asp#:~:text=These%20include%20the%20current%20stock,market%20value%20of%20an%20option) European [Basket options](https://www.investopedia.com/terms/b/basketoption.asp) under [Black-Scholes](https://www.investopedia.com/terms/b/blackscholes.asp) assumptions and compare the results with other traditional numerical solver.




### Steps:

1. Generate and pricing a Basket options data : [Data_Generating](https://github.com/Merhbene/Basket-pricing-using-Neural-Networks/blob/main/Data_Generating.ipynb).
2. Build, train and compare Neural Network model with Monte carlo simulations: [NN_model_for_Basket_Pricing](https://github.com/Merhbene/Basket-pricing-using-Neural-Networks/blob/main/NN_model_for_Basket_Pricing.ipynb)

**In this project:**
* We deal with European basket call.

* We consider 4 asset basket options and 10000 sampels to train the model and we save that in [Basket_pricing_data.csv](https://github.com/Merhbene/Basket-pricing-using-Neural-Networks/blob/main/Basket_pricing_data.csv) file. We can consider any asset numbers since the code is  flexible (For 1 asset case, we set nb_assets=1)

* We consider that asset prices are already weighted.
* We use [Monte-Carlo](https://www.goddardconsulting.ca/option-pricing-monte-carlo-index.html) simulations to compare the performance.


### Conclusion:

The results in NN_model Notebook, shows that, under Black-Scholes assumptions, Neural Network approach reduces the computing time of basket options pricing compared to Monte Carlo approach.

This means, particularly for asset price processes leading to much more
time-consuming computations, that we are able to provide a highly efficient approximation technique
by means of the Neural Networks.

Furthermore, The model accuracy can be further improved, for example, by optimizing the parameters using Grid Search.

Although we focus on European call options that holds the volatility constant in this work, it should be possible to extend the
approach to pricing more complex options, with the Heston stochastic volatility model.






### Bibliography :
* [Machine Learning methods for option pricing and model calibration](https://canopee-group.com/wp-content/uploads/2020/12/Machine-Learning-methods-Coperneec.pdf) 
* [Option Pricing with Deep Learning](https://cs230.stanford.edu/projects_fall_2019/reports/26260984.pdf)
* [Numerical methods for option pricing](https://github.com/shrentseng/Numerical-methods-for-option-pricing/blob/main/Monte%20Carlo%20simulation%20option%20pricing.ipynb)
* [Pricing options and computing implied volatilities
using neural networks](https://arxiv.org/pdf/1901.08943.pdf)



