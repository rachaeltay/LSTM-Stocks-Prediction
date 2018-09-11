# LSTM-Stocks-Prediction

Techinical analysis on various tech stocks to create predictive models. 

After data collection from web scraping, data pre-processing is executed. We used LSTM from the Keras package as our model. Our activation function is relu and optimiser is Adam optimization. The Adam optimization algorithm update network weights iterative based in training data. This gives it an advantage over the classical stochastic gradient. Once the model has been trained, we forecast prices of the tech stocks on particular days.

On top of individual tech stock analysis, we conducted 2 other analysis for comparison.

## 1. Moving Average Convergence Divergence Analysis

MACD analysis provides insight on the momentum and trend of the stock prices. In certain cases, a divergence can be spotted, where the MACD and the stock prices go in opposite direction, and a trend reversal is expected. Generally, we look out for three areas, namely, the MACD zero crossover, MACD and signal crossover, and divergence as mentioned above. The MACD analysis comprises of the MACD, Exponential Moving Average(EMA) of 26 periods - EMA of 12 periods, and the signal, EMA of 9 periods. As in the MACD zero crossover, the further away MACD value is from the zero line, the stronger the momentum of the trend. Positive values of MACD reflects an upwards trend, and vice versa. Next, MACD and signal crossover signifies long and short of the stock, for when MACD > Signal and MACD < Signal respectively. We used these techniques to complement other technical analysis and the neural network prediction to strengthen the confirmation of an upwards trend. The Crossover chart illustrates (MACD - Signal) values.

## 2. Bollinger Bands

Bollinger Bands provides the boundaries of the stock prices, indicating long or short when the prices exceed on either side. The middle line is calculated using the 20-day MA, and the boundaries are determined by adding and subtracting (20-day SD) x 2. Additionally, "the squeeze" is a strong indicator that there is future volatility. It is identified by the closing up of the bands, where volatility within this range is low. At this point, there is a strong calling for an entry into the market, and the direction can be estimated using the 20-day MA trend.
