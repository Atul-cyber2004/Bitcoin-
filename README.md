# Bitcoin
Bitcoin price prediction and analysis

In this project, we'll predict the future price of Bitcoin. We'll use historical data on the price of Bitcoin, along with data from Wikipedia about edits to the Bitcoin page. We'll merge and combine this data, then use it to train a random forest model that will tell us if Bitcoin prices will increase or decrease tomorrow. We'll then switch to an XGBoost model and better predictors to improve accuracy.

We'll develop a backtesting system and use a robust error metric so we can tell if the algorithm is performing well.

This project can be extended to other cryptocurrencies as well.

File overview:
prediction.ipynb - a Jupyter notebook that contains the code to predict Bitcoin prices
sentiment.ipynb - a Jupyter notebook that creates our wikipedia edit dataset.

Data
Computing the Wikipedia edit data takes time. It can be faster to use the version that's already been generated. It's in this repository, and called wikipedia_edits.csv.

We'll be downloading the Bitcoin price data using the yfinance package as part of the project.

Running
First, run the code in sentiment.ipynb to generate a new Wikipedia edits dataset. The dataset committed in the repo is old, and this will get the edits up to the present day.

Second, run the code in prediction.ipynb. By default, this will load data from an existing btc.csv file. Removing that code will ensure that it downloads the newest data from Yahoo Finance.
