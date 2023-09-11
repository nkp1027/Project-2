# Project-2
Project 2
## Proposal
Our project is to train a logistic regression model to make trading predictions for NVIDIA. We will back test and compare it to an SVM model and evaluate the performance by comparing the two. We will be adding new criteria for the buy and sell indicators using the TA library. These include RSI and Ichimoku cloud. Ichimoku cloud helps determine the direction, momentum and support-resistance levels. RSI is the relative strength index which is a momentum oscillator that measures the speed and change of price movements. The source of the data we will be using will be from YahooFinance. 
## Project Members
Nipun, Exzavier, Jeff
## Title
Algorithmic Trading for NVDA
## Project Description
Our project will start with training a logistic regression model to NVDA stock data pulled from YFinance. We will be calculating the daily returns using the closing prices, defining short and long windows (50 and 100 respectively) to calculate the SMA. Once this is done we will then create buy and sell signals as well as training the model to identify those buy and sell signals based on our set parameters. After we train the data we will scale it and create a classification report to determing accuracy of the model we are using. All that which we have done up to this point will lead us to evaluate the model's ability to predict trading signals for the test data. Once the accuracy is shown to us in the classification report for this, we will calculate and plot the cumulative returns for the actual and trading algorithm returns. This is where the logistic regression model will come in, were will will predict the trade signals for the trained data and generate another classification report to determine it's accuracy. Now that this is all done, we will compare the logistic regression to the SVM to determine if there were any changes in the accuracy of predicting.
The new technology we used in this project is the Ichimoku Cloud and RSI indicators to help with predicting buy and sell signals. We pull the data as before and plot the close price in a chart to visualize it. RSI will be calculated using the pulled data and the Ichimoku cloud will be created by adding in the 5 lines of Tenkan, Kijun, Senkou span A, Senkou span B and Chikou Span B. Now we must generate trading signals and visualize the buy and sell points on a graph. After the calculation of the daily returns and strategy returns, we will plot the cumulative returns and plot the Ichimoku Cloud part of the code to visualize the buy and sell points.
## Datasets Used
Historical NVDA stock data from Yahoo Finance
## Team Task Breakdown
Since we are using one data set, we will all be working together to research and implement the new indicators as well as apply what we learned in class to compare the logistic regression model to the SVM model.
## Findings
Based on the classification reports generated for this project we determined that using two tools of the same type is not the optimal way to predict buy and sell signals. The SVM was worse at predicting sell signals and only 1% higher at predicting buy signals. The logistic regression model was 11% better at predicting sell signals yet. This is why we wanted to explore new methods of predicting buy and sell signals using the RSI and Ichimoku cloud which will be displayed in the presentation.
## Installations
To install yfinance you must 'pip install yfinance'
For the Ichimoku Cloud and RSI you must import the TA library by 'import talib' but first you need to make sure it is installed. To install it you must use '$ conda install -c conda-forge ta-lib' in the gitbash terminal.
