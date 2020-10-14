# Capstone-Two

# Introduction:

# 1. The Problem:
  Traders in financial markets typically use charts and 'technical indicators' to indentify entry and exit points. These 'technical indicators' are generally derivatives of price and/or volume, and after having used them for many years I have come to believe that most work only some of the time, some are horrible and some are very useful. Here I will explore using machine learning to test whether there is any predictive power to a confluence of these indicators, and I will also empirically test the usefulness of the indicators that I believe to be reliable, to see if I am indeed correct.
# 2. The Data:
[Data acquisition and wrangling report](https://github.com/londonjevans/Capstone-Two/blob/master/Capstone%20Two%20Data%20acquisition%20and%20wrangling.ipynb)

  I have been collecting intraday trading data for Bitcoin vs USD from Tiingo with a frequency of 1 minute for about 6 weeks, and as of the 14th of October 2020 that amounted to about 95,000 rows of data. A huge benefit of financial data is that it is generally very clean, so there was not a huge amount of work to do on this front, [with very little pre-processing necessary](https://github.com/londonjevans/Capstone-Two/blob/master/Capstone%20Two%20Preprocessing.ipynb).  I also downloaded daily price data, but for Bitcoin this amounts to under 3,000 rows of data, so I will initially be analysing the daily data.
# 3. The Question of Interest:
  I have calculated a reward metric which is a figure that risk-adjusts the overall profit on a trade, by dividing the profit by the maximum drawdown during the holding period. I have initially made the trade holding period 5 minutes, but will eventually explore many different timeframes. I will add a large range of technical indicators as features to the dataset, and then explore whether they have predictive power in predicting reward as y.
# 4. EDA:
 [EDA report](https://github.com/londonjevans/Capstone-Two/blob/master/Capstone%20Two%20EDA.ipynb)
 !(/Users/josevans/Desktop/Screenshot 2020-10-14 at 14.23.29.png)
