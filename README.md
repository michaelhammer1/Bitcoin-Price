# Bitcoin-Price

## Bitcoin Volatility Prediction

By: Michael Hammer

#Overview: Predicting financial asset price moves using machine learning is difficult given these assets tend to move in a brownian motion type fashion. However, as an options trader, predicting future volatility from past realized volatility should have predictive value and assist volatility firms in making money in the bitcoin options market.

## Goal
Use historical daily abosolute volatility to predict future volatility. Use a LSTM model. Ensure that the model is predictive. Ensure that the model is catching the 'weekend effect' where realized volatility comes off every 7 days. 

## Data
Bitstamp has an API where we can pull data at a frequency and time frame as necassary. Given volatility is tradeable as a daily contract, we do not go for a lower frequency. We begin pulling data from September 2017 as before that crypto was really a niche market where the data is likely less relevant to our model.

## Methods
We started by pulling the data. 

Then we visualized the time series of volatility per day and pulled the most volatile days in the dataset.

Finally we modeled future volatility based on our data. We built an Arema model and then feed forward nueral net. We then built the model we expect to be most predictive, the LSTM model.

## Results
The LSTM model was the best model, but still shows poor results with what looks like too much noise. **After hyperparameter tuning...**

## Conclusions


## Next steps
Build a multivariate model where we can input funtions such as where the market is pricing forward volatilities. Add day of the week. Add data around macro events such as FOMC/CPI releases. 
