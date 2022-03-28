# Machine Learning Stock Predicting Notebook

This Jupyter Notebook is used to predict future price of stocks and cryptocurrencies by utilizing machine learning.

## Technologies and libraries

•	pandas – to analyze and manipulate data
•	Random – generates a random float uniformly in the semi-open range
•	NumPy – to operate on large collection of high-level mathematical functions
•	Statsmodels API – to easily develop rapid trading algo
•	sklearn – features various classification, regression and clustering algorithms including support-vector machines, random forests, gradient
boosting, k-means and DBSCAN
•	hvplot – for user-friendly interactive plotting

### Instructions for Machine learning Price Prediction

Installation:

	Open in Colab

•	pip install hvplot
•	pip install datetime
•	pip install autots
•	pip install plotly

Imports:

• import pandas as pd
•import numpy as np
•from pathlib import Path
•import hvplot.pandas
•import matplotlib.pyplot as plt
•from sklearn import svm
•from sklearn.preprocessing import StandardScaler
•from pandas.tseries.offsets import DateOffset
•from sklearn.metrics import classification_report
•import pandas as pd
•import yfinance as yf
•import datetime
•from datetime import date, timedelta
 
#### Collect the latest Google Price data from Yahoo Finance, using yfinance API

data = yf.download('Goog', 
                      start=start_date, 
                      end=end_date, 
                      progress=False)

* can change to any stock or crypto symbol that reports on yahoo finance. 
  Example: 'BTC-USDT'

##### Data.shape

In the above code, we have collected the latest data of Google for the past 730 days and have prepared it for any data science task. Now, let's have a look at the shape of this dataset to see if we are working with 730 rows or not.

###### Visualize the change

Visualize the change in Google to date by using a candlestick chart.

####### Forecast = Prediction 

Using Auto Ts Library to predict the Google price for the net 30 days:

######## Analyze the findings 

Play with the numbers of days and dial in the intent.

######### Compare and test Machine Learning Models

There are several machine learning models included in this notebook to compare and test.