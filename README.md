# DeepLearning_GenAI- Time Series Forecasting-  A Deep Learning Approach to JPMorgan Stock Prediction

[![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?logo=tensorflow&logoColor=white&style=flat)](https://www.tensorflow.org/)
[![Keras](https://img.shields.io/badge/Keras-D00000?logo=keras&logoColor=white&style=flat)](https://keras.io/)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?logo=numpy&logoColor=white)




![image alt](https://github.com/x23425237/DeepLearning_GenAI/blob/main/DeepLearning.jpg)
<img src="https://github.com/x23425237/DeepLearning_GenAI/blob/main/formula_lstm.jpg?raw=true" alt="image alt" width="400"/>


Time series forecasting has evolved since George Udall
Yule first developed Autoregressive models(ARIMA) in 1920
[8]. Moving average and Exponential smoothing(Holt-Winters)
are among the oldest methods still actively used due to their
simplicity and implementation on medium to small datasets.
To address the challenges in forecasting stock prices, for
example, Non-linearity in the stock prices, Data volume,
and due to the dynamic nature of the financial market, where
stock prices are highly influenced by the economic indicators,
market sentiments, events, and news, several deep learning
Models such as LSTM, GRU and RNN were invented in late
20th Century. These models are equipped with understanding-
ing complex patterns and non-linearities which proved to be
challenging for traditional methods to address.
JPMorgan Chase & Co, one of the world’s largest bank,
American multinational financial service company that has
its UK headquarters in London. The bank has a significant presence-
ence and operations in Ireland, providing advisory services
for investment banking, Asset management, and fund
Administration. For a stock analyst understanding stock perfor-
Performance could provide insights into the company’s investment
opportunities and its financial market position
a) Objective: The objective of this experiment is to
Compare the effectiveness of traditional time series models
such as Moving Average models and deep learning models
such as Recurrent Neural Networks(RNN), Long short-
Term Memory(LSTM) on JPMorgan daily(5min) stock
prices. Fine-tune the models to obtain minimum Absolute
Mean Square Error(AME).


# EDA-JPM-StockPrices(5min)- Closing Price

![image alt](https://github.com/x23425237/DeepLearning_GenAI/blob/main/eda_old.jpg)

# Methodology- Time Series 

JPMorgan Daily(5min) stock prices are taken from Alpha
Vantage, which provides real-time and historical financial market-
ket data through data APIs. Daily JPM data consists of 4,120
points, Prices are collected every 5 min, fetching the most
recent stock prices. The daily dataset consists of 3,375 price
changes for March and 745 for February. As the Real time data
fetches only the most recent 30-day records, another dataset
that contains historic monthly stock prices from Kaggle is used
for this paper. Historical monthly data AIG.csv dataset from
Kaggle is used. Historic data contains 12,793 monthly stock
prices from Year 1973-2023. The reason behind using two
separate datasets is to compare the predictive capabilities of
deep learning models, where stock prices are recorded more
frequently than monthly which contains only 12 data points
in a year. There is a high level of detail is captured in daily
stock prices when compared to monthly. There is a high level
of fluctuations and Volatility in the daily prices than in the monthly.
Deep learning models such as LSTM are capable of capturing
long-term dependencies and can remember information from
an earlier point in the day when compared to traditional models
which give less importance to long-term patterns. 

# Model Evaluation- Deep Learning 
![image alt](https://github.com/x23425237/DeepLearning_GenAI/blob/main/Loss-Rnn.jpg)

![image alt](https://github.com/x23425237/DeepLearning_GenAI/blob/main/LSTM_and_GRU.jpg)

> **Note:** During model training- output is recorded in finial_results.xlsx.


