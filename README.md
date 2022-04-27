# Basket pricing using Neural Networks

### Challange:

The client wants to explore novel methodologies for accelerating the pricing of exotic derivatives. 

### Goal: 

The goal is to build a neural network model for [pricing](https://www.investopedia.com/articles/optioninvestor/07/options_beat_market.asp#:~:text=These%20include%20the%20current%20stock,market%20value%20of%20an%20option) European [Basket options](https://www.investopedia.com/terms/b/basketoption.asp) under [Black-Scholes](https://www.investopedia.com/terms/b/blackscholes.asp) assumptions and compare the prices with [Monte-Carlo](https://www.goddardconsulting.ca/option-pricing-monte-carlo-index.html) simulations.


### Steps:

1. Generate and pricing a Basket options data : [Data_Generating](https://github.com/Merhbene/Basket-pricing-using-Neural-Networks/blob/main/Data_Generating.ipynb).
2. Build, train and compare Neural Network model with Monte carlo simulations [NN_model_for_Basket_Pricing](https://github.com/Merhbene/Basket-pricing-using-Neural-Networks/blob/main/NN_model_for_Basket_Pricing.ipynb)

**In this project:**
* We deal with European basket call.

* We consider 4 asset basket options and 10000 sampels to train the model and we save that in [Basket_pricing_data.csv](https://github.com/Merhbene/Basket-pricing-using-Neural-Networks/blob/main/Basket_pricing_data.csv) file. We can consider any asset numbers since the code is  flexible.

* We consider that asset prices are already weighted.

### Bibliography :
* [Machine Learning methods for option pricing and model calibration](https://canopee-group.com/wp-content/uploads/2020/12/Machine-Learning-methods-Coperneec.pdf) 
* [Option Pricing with Deep Learning](https://cs230.stanford.edu/projects_fall_2019/reports/26260984.pdf)
* [Numerical methods for option pricing](https://github.com/shrentseng/Numerical-methods-for-option-pricing/blob/main/Monte%20Carlo%20simulation%20option%20pricing.ipynb)



