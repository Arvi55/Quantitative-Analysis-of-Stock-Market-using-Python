#  📊Project Background

Quantitative Analysis in the stock market involves the use of mathematical and statistical techniques to understand, predict, and make decisions about financial investments. If you want to learn how to perform Quantitative Analysis on stock market data, this article is for you. In this article, I’ll take you through the task of Quantitative Analysis of the stock market using Python.




#  Quantitative Analysis of Stock Market:
Quantitative Analysis in the stock market is a financial methodology that utilizes mathematical and statistical techniques to analyze stocks and financial markets.

Below is the process we can follow for the task of Quantitative Analysis of the stock market:

- Clearly define the objectives and questions to be answered.
- Identify the key performance indicators (KPIs) relevant to the analysis.
- Gather historical stock market data, including prices, volumes, and other relevant financial indicators.
- Clean and preprocess the data to handle missing values, outliers, and errors.
- Conduct initial analysis to understand data distributions, patterns, and correlations.
- Implement various strategies based on quantitative analysis.

To get started with this task, we need appropriate data. I found an ideal dataset for this task. 

You can download the dataset from [HERE.](https://github.com/Arvi55/Quantitative-Analysis-of-Stock-Market-using-Python/blob/main/stocks.csv)

# Data Structure & Initial Checks

The dataset contains the following columns for stock market data:

- Ticker: The stock ticker symbol.
- Date: The trading date.
- Open: The opening price of the stock for the day.
- High: The highest price of the stock during the day.
- Low: The lowest price of the stock during the day.
- Close: The closing price of the stock for the day.
- Adj Close: The adjusted closing price, which accounts for all - corporate actions such as dividends, stock splits, etc.
- Volume: The number of shares traded during the day.
![App Screenshot](https://github.com/Arvi55/Quantitative-Analysis-of-Stock-Market-using-Python/blob/main/Dataset.png?raw=true)



# Executive Summary


**Overview of Findings**

To perform a quantitative analysis, we can explore various statistical concepts like descriptive statistics, time series analysis, correlation analysis, and more. Here are some potential analyses we can perform:

- Descriptive Statistics: Summary statistics (mean, median, standard deviation, etc.) for each stock.
- Time Series Analysis: Trends and patterns over time, especially for closing prices.
- Volatility Analysis: How much the stock price fluctuates over a period.
- Correlation Analysis: How stock prices of different companies are related to each other.
- Comparative Analysis: Comparing the performance of different stocks.
- Risk-Return Trade-off Analysis: Analyzing the balance between the potential risks and rewards of different stocks, aiding in portfolio management.



# Descriptive Statistics:

   Let’s break down the results for each stock:

**AAPL (Apple Inc.)**

- Count: 62.0 (The number of observations or trading days included in the dataset for AAPL)
- Mean: 158.24 (The average closing price)
- Standard Deviation: 7.36 (Measures the amount of variation or dispersion of closing prices)
- Minimum: 145.31 (The lowest closing price in the dataset)
  25th Percentile: 152.08 (25% of the closing prices are below this value)
- Median (50%): 158.06 (The middle value of the closing prices)
  75th Percentile: 165.16 (75% of the closing prices are below this value)
- Maximum: 173.57 (The highest closing price in the dataset)
**GOOG (Alphabet Inc.)**

Similar statistics as AAPL, but for GOOG. The mean closing price is 100.63, with a standard deviation of 6.28, indicating less variability in closing prices compared to AAPL.

**MSFT (Microsoft Corporation)**

The dataset includes the same number of observations for MSFT. It has a higher mean closing price of 275.04 and a higher standard deviation of 17.68, suggesting greater price variability than AAPL and GOOG.

**NFLX (Netflix Inc.)**

NFLX shows the highest mean closing price (327.61) among these stocks and the highest standard deviation (18.55), indicating the most significant price fluctuation.



   ![App Screenshot](https://github.com/Arvi55/Quantitative-Analysis-of-Stock-Market-using-Python/blob/main/Descriptive%20Statistics.png?raw=true)


 # Time Series Analysis

Next, we’ll proceed with the Time Series Analysis to examine trends and patterns over time, focusing on the closing prices:.

The below plot displays the time series of the closing prices for each stock (AAPL, GOOG, MSFT, NFLX) over the observed period. Here are some key observations:

- Trend: Each stock shows its unique trend over time. For instance, AAPL and MSFT exhibit a general upward trend in this period.
- Volatility: There is noticeable volatility in the stock prices. For example, NFLX shows more pronounced fluctuations compared to others.
- Comparative Performance: When comparing the stocks, MSFT and NFLX generally trade at higher price levels than AAPL and GOOG in this dataset.

   ![App Screenshot](https://github.com/Arvi55/Quantitative-Analysis-of-Stock-Market-using-Python/blob/main/time%20series.png?raw=true)


 # Volatility Analysis

Next, let’s focus on Volatility Analysis. We’ll calculate and compare the volatility (standard deviation) of the closing prices for each stock. It will give us an insight into how much the stock prices fluctuated over the period:

The bar chart and the accompanying data show the volatility (measured as standard deviation) of the closing prices for each stock. Here’s how they rank in terms of volatility:

- NFLX: Highest volatility with a standard deviation of approximately 18.55.
- MSFT: Next highest, with a standard deviation of around 17.68.
- AAPL: Lower volatility compared to NFLX and MSFT, with a standard deviation of about 7.36.
- GOOG: The least volatile in this set, with a standard deviation of approximately 6.28.

It indicates that NFLX and MSFT stocks were more prone to price fluctuations during this period compared to AAPL and GOOG.

![Alt1](https://github.com/Arvi55/Quantitative-Analysis-of-Stock-Market-using-Python/blob/main/volatility.png?raw=true) 

 
# Correlation Analysis

Next, we’ll perform a Correlation Analysis to understand how the stock prices of these companies are related to each other:

The heatmap below displays the correlation matrix of the closing prices of the four stocks (AAPL, GOOG, MSFT, NFLX). Here’s what the correlation coefficients suggest:

- Values close to +1 indicate a strong positive correlation, meaning that as one stock’s price increases, the other tends to increase as well.
- Values close to -1 indicate a strong negative correlation, where one stock’s price increase corresponds to a decrease in the other.
- Values around 0 indicate a lack of correlation.
From the heatmap, we can observe that there are varying degrees of positive correlations between the stock prices, with some pairs showing stronger correlations than others. For instance, AAPL and MSFT seem to have a relatively higher positive correlation.

 ![Alt1](https://github.com/Arvi55/Quantitative-Analysis-of-Stock-Market-using-Python/blob/main/correlation%20matrix.png?raw=true) 

 

# Comparative Analysis

Now, let’s move on to Comparative Analysis. In this step, we’ll compare the performance of different stocks based on their returns over the period. We’ll calculate the percentage change in closing prices from the start to the end of the period for each stock:

The bar chart and the accompanying data show the percentage change in the closing prices of the stocks from the start to the end of the observed period:

- MSFT: The highest positive change of approximately 16.10%.
- AAPL: Exhibited a positive change of approximately 12.23%. It indicates a solid performance, though slightly lower than MSFT’s.
- GOOG: Showed a slight negative change of about -1.69%. It indicates a minor decline in its stock price over the observed period.
- NFLX: Experienced the most significant negative change, at approximately -11.07%. It suggests a notable decrease in its stock price during the period.

![Alt1](https://github.com/Arvi55/Quantitative-Analysis-of-Stock-Market-using-Python/blob/main/percentage%20change.png?raw=true) 

# Daily Risk Vs. Return Analysis
To perform a Risk vs. Return Analysis, we will calculate the average daily return and the standard deviation of daily returns for each stock. The standard deviation will serve as a proxy for risk, while the average daily return represents the expected return.

We will then plot these values to visually assess the risk-return profile of each stock. Stocks with higher average returns and lower risk (standard deviation) are generally more desirable, but investment decisions often depend on the investor’s risk tolerance:

 - So, AAPL shows the lowest risk combined with a positive average daily return, suggesting a more stable investment with consistent returns. GOOG has higher volatility than AAPL and, on average, a slightly negative daily return, indicating a riskier and less rewarding investment during this period.

- MSFT shows moderate risk with the highest average daily return, suggesting a potentially more rewarding investment, although with higher volatility compared to AAPL. NFLX exhibits the highest risk and a negative average daily return, indicating it was the most volatile and least rewarding investment among these stocks over the analyzed period
![Alt1](https://github.com/Arvi55/Quantitative-Analysis-of-Stock-Market-using-Python/blob/main/risk%20vs%20return.png?raw=true)

# Result

 
- **Highest Performing Stock:-**
  
  🟢Microsoft (MSFT) delivered the best return with a +16.10% price increase over the period.

- **Most Volatile Stock:-**
  
  🔴 Netflix (NFLX) showed the highest volatility with a standard deviation of 18.55, making it the riskiest stock.

- **Safest Stock (Risk-Return Balance):-**
   
   ✅ Apple (AAPL) had the lowest daily risk with a standard deviation of 7.36 and a positive return of +12.23%, suggesting stable growth.

- **Strongest Correlation:-**
  
  🔗 The highest positive correlation was observed between AAPL and MSFT, indicating their prices tend to move together.

- **Worst Performing Stock:-**

  🔻 Netflix (NFLX) recorded the largest decline with a -11.07% drop in price and negative average daily return, despite having the highest mean price.








