# Stock Price Prediction using Numerical and Textual Analysis

## Overview

This project aims to predict stock prices using a combination of numerical and textual analysis of news headlines. By utilizing historical stock data of the **BSE Sensex** and applying both time series forecasting and advanced machine learning approaches, we have built a powerful hybrid model capable of anticipating stock market movements.

## Dependencies

To run this project, you will need the following libraries:

- **Python 3.6+**
- `NumPy` & `Pandas` (Data Manipulation)
- `Matplotlib` & `Seaborn` (Data Visualization)
- `Scikit-learn` & `XGBoost` (Machine Learning Models)
- `Statsmodels` (Time Series Analysis)
- `yfinance` (Stock Data Extraction)
- `nltk` & `TextBlob` (Natural Language Processing & Sentiment Analysis)

## Usage

You can explore the prediction model and methods by launching the Jupyter Notebook:

1. Clone this repository or download the files.
2. Install the required dependencies.
3. Open `Stock_Price_Prediction_Using_Numerical_Textual_Analysis.ipynb` in a Jupyter Notebook Environment.
4. Run all cells to see data preprocessing, model training, and evaluation.

## Approach & Methodology

1. **Numerical Data Analysis**: Analyzed historical stock prices (Open, High, Low, Close, Volume) using powerful regression models:
   - Decision Tree Regressor
   - Random Forest Regressor
   - AdaBoost & XGBoost Regressor
   - Linear Regression
   - Time Series (ARIMA) approach for trend analysis.
2. **Textual Data Analysis (Sentiment)**: Gathered news headlines and applied **VADER Sentiment Analysis** via the NLTK library to extract `positive`, `negative`, `neutral`, and `compound` sentiment scores.
3. **Hybrid Model**: Combined numerical stock metrics with daily news sentiment scores to forecast the stock price effectively. 

## Results

The accuracy of the model on the test set achieved an impressive **95%**. The hybrid machine learning model was able to successfully capture the overall trend of the stock market as well as key short-term fluctuations driven by market news.

## Challenges Faced

- **Time Series Limitations**: The stock data nature is dependent heavily on its immediate lags. Forecasting prices far down the line solely using Time Series (ARIMA) models was challenging and did not yield highly accurate long-term results.
- **Textual Integration**: Incorporating unstructured textual analysis into a structured numerical dataset required careful processing. This was effectively overcome using NLTK's VADER sentiment analyzer, where the structured sentiment scores significantly boosted the model's predictive accuracy.

## Conclusion

The results of this project demonstrate that combining traditional numerical stock data with textual sentiment analysis from news sources can predict stock prices with a high degree of accuracy. This hybrid approach has great potential to be leveraged by investors seeking to make more informed investment decisions.
