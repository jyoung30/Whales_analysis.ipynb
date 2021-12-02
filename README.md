# Whales_analysis.ipynb
![portfolio-analysis](https://user-images.githubusercontent.com/71282811/144494459-e722465f-a374-4500-8345-dc27ad81a500.png)
Background

Harold's company has been investing in algorithmic trading strategies. Some of the investment managers love them, some hate them, but they all think their way is best.

You just learned these quantitative analysis techniques with Python and Pandas, so Harold has come to you with a challenge—to help him determine which portfolio is performing the best across multiple areas: volatility, returns, risk, and Sharpe ratios.

You need to create a tool (an analysis notebook) that analyzes and visualizes the major metrics of the portfolios across all of these areas, and determine which portfolio outperformed the others. You will be given the historical daily returns of several portfolios: some from the firm's algorithmic portfolios, some that represent the portfolios of famous "whale" investors like Warren Buffett, and some from the big hedge and mutual funds. You will then use this analysis to create a custom portfolio of stocks and compare its performance to that of the other portfolios, as well as the larger market (S&P 500 Index).

For this homework assignment, you have three main tasks:

Read in and Wrangle Returns Data

Determine Success of Each Portfolio

Choose and Evaluate a Custom Portfolio

Instructions
File: Whale Analysis Starter Code

Prepare the Data
First, read and clean several CSV files for analysis. The CSV files include whale portfolio returns, algorithmic trading portfolio returns, and S&P 500 historical prices. Use the Whale Analysis Starter Code to complete the following steps:

Use Pandas to read the following CSV files as a DataFrame. Be sure to convert the dates to a DateTimeIndex.

whale_returns.csv: Contains returns of some famous "whale" investors' portfolios.

algo_returns.csv: Contains returns from the in-house trading algorithms from Harold's company.

sp500_history.csv: Contains historical closing prices of the S&P 500 Index.

Detect and remove null values.

If any columns have dollar signs or characters other than numeric values, remove those characters and convert the data types as needed.

The whale portfolios and algorithmic portfolio CSV files contain daily returns, but the S&P 500 CSV file contains closing prices. Convert the S&P 500 closing prices to daily returns.

Join Whale Returns, Algorithmic Returns, and the S&P 500 Returns into a single DataFrame with columns for each portfolio's returns.

returns-dataframe.png

Conduct Quantitative Analysis
Analyze the data to see if any of the portfolios outperform the stock market (i.e., the S&P 500).

Performance Analysis
Calculate and plot daily returns of all portfolios.

Calculate and plot cumulative returns for all portfolios. Does any portfolio outperform the S&P 500?

Risk Analysis
Create a box plot for each of the returns.

Calculate the standard deviation for each portfolio.

Determine which portfolios are riskier than the S&P 500.

Calculate the Annualized Standard Deviation.

Rolling Statistics
Calculate and plot the rolling standard deviation for all portfolios using a 21-day window.

Calculate and plot the correlation between each stock to determine which portfolios may mimick the S&P 500.

Choose one portfolio, then calculate and plot the 60-day rolling beta between it and the S&P 500.

Rolling Statistics Challenge: Exponentially Weighted Average
An alternative method to calculate a rolling window is to take the exponentially weighted moving average. This is like a moving window average, but it assigns greater importance to more recent observations. Try calculating the ewm with a 21-day half-life.

Sharpe Ratios
Investment managers and their institutional investors look at the return-to-risk ratio, not just the returns. After all, if you have two portfolios that each offer a 10% return, yet one is lower risk, you would invest in the lower-risk portfolio, right?

Using the daily returns, calculate and visualize the Sharpe ratios using a bar plot.

Determine whether the algorithmic strategies outperform both the market (S&P 500) and the whales portfolios.

Create a Custom Portfolio
Harold is ecstatic that you were able to help him prove that the algorithmic trading portfolios are doing so well compared to the market and whales portfolios. However, now you are wondering whether you can choose your own portfolio that performs just as well as the algorithmic portfolios. Investigate by doing the following:

Visit Google Sheets and use the built-in Google Finance function to choose 3-5 stocks for your portfolio.

Download the data as CSV files and calculate the portfolio returns.

Calculate the weighted returns for your portfolio, assuming equal number of shares per stock.

Add your portfolio returns to the DataFrame with the other portfolios.

Run the following analyses:

Calculate the Annualized Standard Deviation.
Calculate and plot rolling std with a 21-day window.
Calculate and plot the correlation.
Calculate and plot beta for your portfolio compared to the S&P 60 TSX.
Calculate the Sharpe ratios and generate a bar plot.
How does your portfolio do?
