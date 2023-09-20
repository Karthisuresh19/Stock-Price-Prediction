# Stock-Price-Prediction
Stock Price Prediction using Numerical and Textual Analysis

Overview

This project aims to predict stock prices using a combination of numerical and textual analysis of the news headlines. The project uses the historical stock data of BSE Sensex and applies both time series and machine learning approaches.

Dependencies

Python 3.6+
NumPy
Pandas
Matplotlib
Scikit-learn
Statsmodel

Usage

To get the notebook and run it, you can download it or clone the repository and run it in the Jupyter Notebook Environment.


Results

The accuracy of the model on the test set is 95%. The model was able to capture the overall trend of the stock market, as well as some of the short-term fluctuations.

Challenges

One of the challenges faced during the project was dealing with nature of the data which is dependendent only its immediate lags. Such nature does not allow to forecast the price more days down the line. Time Series (ARIMA) approach to this problem was a bit challenging and the model didn't do much

Another challenge was incorporating textual analysis into the model. To overcome this challenge, a sentiment analysis was done by making use of the VADER in the NLTK library. The news headines would be passed and it would return a dict containing pos, neg, neu and compound. Eventually, the information of the sentiment scores helped in improving the model's accuracy.

Conclusion

The results of this project show that it is possible to use a combination of numerical and textual analysis to predict stock prices with a high degree of accuracy. This approach has the potential to be used by investors to make more informed decisions about their investments.
