# S&P 500 Daily Stock Data Extraction and Analysis

This script is designed to extract daily stock information for the S&P 500 index from the website [Slickcharts](https://www.slickcharts.com/sp500). It gathers the daily stock data, including stock names, tickers, and other relevant metrics, and creates a structured dataset for further analysis.

## Features

- **Web Scraping**: The script uses Python libraries like `requests` and `BeautifulSoup` to scrape real-time stock data from the S&P 500 table.
  
- **Data Processing**: The script extracts the stock data from the table and organizes it into a pandas DataFrame.
  
- **Date Assignment**: Each extracted stock data entry is tagged with today's date for easy tracking of daily stock changes.

## Libraries Used

- **requests**: Used to send HTTP requests to the website and retrieve the HTML content.
  
- **BeautifulSoup**: Used for parsing the HTML content and extracting relevant data from the table.
  
- **pandas**: Provides the DataFrame structure for storing and analyzing the extracted data.
  
- **datetime**: Used to capture today's date and assign it to the extracted data for proper timestamping.

## Script Flow

1. **Request Data**:  
   The script sends a `GET` request to the S&P 500 data page at [Slickcharts](https://www.slickcharts.com/sp500).

2. **Parse HTML**:  
   The HTML content of the page is parsed using `BeautifulSoup` to find the table containing the stock data.

3. **Extract Data**:  
   The script extracts the table headers and the corresponding stock data (including stock names, tickers, and metrics).

4. **Create DataFrame**:  
   The extracted data is structured into a pandas DataFrame with the appropriate column names.

5. **Date Assignment**:  
   The current date is added as a new column to each row in the DataFrame, allowing for daily tracking.

6. **Data Display**:  
   The DataFrame with today's stock data is displayed for review.

## Example Output

The output DataFrame will contain columns like the following:

```text
      Name          Ticker    Weight       Date
0   Apple Inc.     AAPL      6.5%   2025-04-18
1   Microsoft      MSFT      5.0%   2025-04-18
...
