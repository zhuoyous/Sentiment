
Financial Sentiment Analysis & Stock Trend Prediction
====================================================

This project builds a modular pipeline to collect financial data, perform sentiment analysis on stock-related news, and use this information to predict stock price trends—focusing on the relationship between sentiment scores and VWAP (Volume Weighted Average Price).

Project Structure:
------------------
- Main.ipynb                  : Central orchestration notebook for analysis
- deeper analysis.ipynb      : Deeper statistical evaluation and modeling
- three_stock_analysis.ipynb : Case study on 3 selected stocks
- stock_list_generation.ipynb: Ticker list creation and filtering logic
- test_yahoo_data crawler.ipynb : Yahoo Finance data fetcher
- test_news_crawler.ipynb    : News content collection with GPT sentiment
- test_daily_update.ipynb    : Scheduled data update prototype
- records.csv                : Combined stock sentiment & VWAP dataset
- stock_list.csv             : Ticker list used in analysis
- stock_list.npy             : Serialized NumPy list of stocks

Project Highlights:
-------------------
- Automated Data Collection using Yahoo Finance and news sources
- GPT-Powered Sentiment Scoring on financial news content
- VWAP Trend Modeling to study price movement correlation
- Statistical Testing (ANOVA, correlation) for validation
- Machine Learning Models: Logistic Regression, XGBoost, Random Forest
- Daily Update Simulation with test notebooks

Usage:
------
1. Run stock_list_generation.ipynb to create the ticker universe.
2. Run test_yahoo_data crawler.ipynb to collect price data.
3. Run test_news_crawler.ipynb to gather news and generate sentiment.
4. Analyze merged data in Main.ipynb, deeper analysis.ipynb, and three_stock_analysis.ipynb

Results Summary:
----------------
- Achieved up to around 70% accuracy predicting stock direction using VWAP and sentiment.
- Sentiment shows predictive power over VWAP level, more than VWAP return.
- ANOVA and correlation tests confirm the significance of sentiment signals.

Future Work:
------------
- Integrate technical indicators (RSI, MACD)
- Expand news source coverage
- Improve model accuracy with more data

