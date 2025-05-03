# 📈 S&P 500 Stock Analysis Project

This project extracts, analyzes, and visualizes data from the S&P 500 stock market index using Python. The workflow includes data scraping, transformation, and insightful visualizations.

---

## 📊 Data Collection

- Scrapes S&P 500 data from [slickcharts.com](https://www.slickcharts.com/sp500)
- Saves the data to CSV files with company details, stock price, weight, and performance
- Merges multiple CSV files over time for long-term trend analysis

---

## 🔍 Key Analysis and Visualizations

### 1. 🟢 Top Gainers and 🔴 Losers (Last 14 Days)
- Extracts the top 10 gainers and losers based on percentage change over the last 14 days
- Visualizes results using bar charts  
- 📄 **Notebook:** [`s&p500_top10_gainers_and_losers.ipynb`](./s&p500_top10_gainers_and_losers.ipynb)

---

### 2. 🏢 Top 20 Weight Companies in S&P 500
- Identifies top 20 companies by index weight
- Analyzes stock price volatility (difference between max and min prices)
- Visualizes results with color-coded bar charts  
- 📄 **Notebook:** [`s&p500_top20_weight_comapnies.ipynb`](./s&p500_top20_weight_comapnies.ipynb)

---

### 3. 📉 Stock Price Trends for Top 100 Companies
- Analyzes normalized stock price trends (base = 100) for top 100 companies by average weight
- Visualizes multi-line plots across subplots for better readability  
- 📄 **Notebook:** [`s&p500_top100_stock_price_trends.ipynb`](./s&p500_top100_stock_price_trends.ipynb)

---

## 🛠️ Technologies Used

- Python: `requests`, `pandas`, `BeautifulSoup`
- Visualization: `matplotlib`, `seaborn`
- Jupyter Notebook

---

## 📂 Output

- Cleaned and merged CSV datasets
- Interactive and static data visualizations
- Actionable insights into S&P 500 stock dynamics

---

Feel free to explore the notebooks to see how the analysis was conducted step by step!
