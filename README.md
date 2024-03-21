# Forecasting-Nifty-50-Index-with-News-Sentiments
Forecasting Nifty 50 Index with News Sentiments

## Why Utilize News Sentiments?
Market sentiment measures investors' feelings towards financial markets, impacting price changes and creating trading opportunities for both active and long-term investors. Sentiment analysis research shows a strong link between stock price shifts and news publications. Studies using algorithms like support vector machines, naive Bayes regression, and deep learning demonstrate this correlation. Deep learning effectiveness depends on the amount of training data.

## Project Agenda
• **Data Sourcing**: Loading data from Investing.com and Twitter.

• **Scoring Metric**: Since it is a regression problem, we will be using Root Mean Square Error (RMSE) to compare the performance of various models.

• **Feature Engineering and Data Cleaning**: Did Text Processing and Text Processing and Timestamp Normalization.

• **Exploratory Data Analysis**: Visualized Text and Market Data for Insights.

• **Modelling**: Utilized various models like ARIMA, SARIMAX, LSTM, Prophet.

• **Anomaly Detection**: Error Plots and Graphs for Anomaly Identification.

## Feature Engineering
For tweet preprocessing, the following steps have been implemented:

Removal of hyperlinks starting with "http," "pic.twitter.com," or "https."
Exclusion of special characters, emoticons, hashtags (#), and the "@" symbol.
Elimination of specific words like "ETMarkets," "ndtv," "moneycontrol," "marketsupdate," "biznews," "NewsAlert," and "Click here for LIVE updates."
Extraction of numerical values from the text has been omitted.

Loading Nifty 50 Indices:

![image](https://github.com/MANIMADHURIE/Forecasting-Nifty-50-Index-with-News-Sentiments/assets/37103568/c98c4b24-ae71-4b10-8145-e894b5933011)

Loading Tweets:

![image](https://github.com/MANIMADHURIE/Forecasting-Nifty-50-Index-with-News-Sentiments/assets/37103568/994d49d1-e0ad-4d69-a18e-93be7c95341f)

## Data Preprocessing
Tokenization, stopword removal, and bigram extraction are not required in this case, as we intend to utilize a pre-trained sentiment analyzer, specifically VADER, given that our data is unsupervised.
The selection of VADER is based on its proven effectiveness, particularly in analyzing social media text. Positive Sentiment signifies positive news and Negative Sentiment signifies negative news. Positive news should rise the index prices and vice versa.

## Exploratory Data Analysis
There are no Duplicates and Null values in the data. We can observe that words like gain, top, rise, surge result in a positive tweet and words like lower, fall, hit, drop, slump result in a negative tweet. Looks like bank stocks are the most fluctuating ones.

Word Cloud for Positive Tweets:

![image](https://github.com/MANIMADHURIE/Forecasting-Nifty-50-Index-with-News-Sentiments/assets/37103568/6e95ef55-20f1-4ccc-9223-e78a2d8007af)

Word Cloud for Negative Tweets:

![image](https://github.com/MANIMADHURIE/Forecasting-Nifty-50-Index-with-News-Sentiments/assets/37103568/b4a694f3-46b7-4816-b005-0c671f186c00)

## Sentiment Analysis
For the majority of news, **VADER** is confident in detecting either positive or negative sentiment since most of the points lie on the boundary. This shows accurate and confident prediction from VADER library.

## Modeling

![image](https://github.com/MANIMADHURIE/Forecasting-Nifty-50-Index-with-News-Sentiments/assets/37103568/d83a1e57-d4f9-4b48-ba72-95b5444ec548)

## Conclusion
In this project, I've gained valuable experience in managing and processing time series data, and I've developed deep learning models with a focus on real-world production applications. Notably, I've tackled the formidable task of working with stock price time series data and achieved a high level of accuracy in predicting the Nifty Index data.












