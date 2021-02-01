# Deep-Learning-Homework14
Homework 14

### Which model has a lower loss?

The model with the FNG features has a loss of 0.0688, significantly higher than the loss for the model that using just closing prices (0.0094)


### Which model tracks the actual values better over time?

Based on the LSTM RNN model predictions, the model that does not include Crypto Fear and Greed Index (FNG) features does a better job predicting the value of Bitcoin. The below charts show the better performance of the model withoutthe FNG features, which is expected given the lower loss values. 

![closing_prices_10.png](Images/closing_prices_10.png)
![fng_model_10.png](Images/fng_model_10.png)


### Which window size works best for the model?

For the model that does not use FNG features, the 10 day window model seems to perform better to predict the value of Bitcoin. The model loss estimate is also smaller for the 10 window than for the 30 or 60 day window. The 60 day window, seems to perform bettwe than the 30 days. 

Comparison of charts for closing prices model:
![closing_prices_10.png](Images/closing_prices_10.png) 
![closing_prices_30.png](Images/closing_prices_30.png) 
![closing_prices_60.png](Images/closing_prices_60.png)

For the model using FNG features, increasing the rolling numbers slightly imrpoves the model loss for the 30 day window but performs worse for the 60 days window. In any case, irrespective of the window choice, the model performance is not as accurate as the prior model. 

![fng_model_10.png](Images/fng_model_10.png) 
![fng_model_30.png](Images/fng_model_30.png)
![fng_model_60.png](Images/fng_model_60.png)
