# S&P 500 Stock Analysis Project

This project extracts, analyzes, and visualizes data from the S&P 500 stock market index. The workflow includes the following steps:

## Data Collection
- Scrapes S&P 500 data from [slickcharts.com](https://www.slickcharts.com/sp500).
- Saves the data to CSV files with company details, stock price, weight, and performance.
- Merges multiple CSV files over time for long-term analysis.

## Key Analysis and Visualizations

### 1. Top Gainers and Losers (Last 14 Days)
- Extracts the top 10 gainers and losers from the last 14 days based on percent change.
- Visualizes the results in bar charts.

### 2. Top 20 Weight Companies in S&P 500
- Identifies the top 20 companies by index weight.
- Analyzes the price trends and computes the difference between their minimum and maximum stock prices.
- Visualizes the companies with color-coded bars representing price volatility.

### 3. Stock Price Trends for Top 100 Companies
- Analyzes the stock price trends for the top 100 S&P 500 companies by average weight.
- Normalizes stock prices (base = 100 at the first available date) and visualizes the trends over time across multiple subplots.

## Technologies Used:
- Python (Requests, Pandas, BeautifulSoup)
- Data Visualization (Matplotlib, Seaborn)

## Output:
- CSV files for stock data and analysis results.
- Interactive visualizations displaying stock trends and performance.
