Financial Data Extractor and Reporter 
README
 Introduction
 This project is a Financial Data Extractor and Reporter built using Google Colab,
 Matplotlib, and the Google Gemini API. It automatically fetches historical stock price
 data (or cryptocurrency data with minimal changes), visualizes the trend, and
 generates a plain-English market summary.
 By default, it analyzes Tesla (TSLA) stock for the past year, but it can be customized
 for any valid ticker symbol.
 Features
 Fetches the last 1 year of historical stock data from Yahoo Finance using the
 yfinance API.
 Automatically handles missing or invalid ticker inputs.
 Generates a closing price trend chart using Matplotlib.
 Produces an AI-generated plain-English summary of the price trend using Google
 Gemini 1.5 Flash.
 Customizable for any stock or cryptocurrency ticker symbol.
 Designed for educational purposes only — no financial predictions or advice.
 Tech Stack
 Python
 Google Colab
 Matplotlib (for charting)
 Pandas (for data handling)
 yfinance (for fetching stock data)
 Google Gemini API (
 gemini-1.5-flash )
 Datetime (for date range management)
 How It Works
 1. The user runs the script in Google Colab or a Python environment.
 2. The program fetches the last 365 days of historical price data for the
 specified ticker.
 3. Data is visualized as a closing price trend chart.
 4. Key price statistics are calculated:
 Starting Price
 Final Price
 Highest Price
 Lowest Price
 5. A prompt is sent to Google Gemini 1.5 Flash, which generates a short, plain
English summary.
 6. The report is printed in the console along with the chart.
 7. To change the stock ticker from Tesla (TSLA) to another:
 Open the script in Colab or your code editor.
Locate the line:
 ticker_symbol = 'TSLA'
 Replace 
'TSLA' with the ticker symbol of your choice. For example:
 Apple Inc. → 
'AAPL'
 Microsoft Corp. → 
'MSFT'
 Amazon.com Inc. → 
'AMZN'
 Save the script and rerun it.
 The program will now fetch, chart, and summarize the selected stock’s
 data.
 Requirements
 Python 3.8+
 Google Colab environment or local Python setup
 yfinance library
 Matplotlib
 Pandas
 Google Generative AI Python SDK
 A valid Google Gemini API key
 Setup Instructions
 1. Open the project in Google Colab or your local Python environment.
 2. Install necessary libraries:
 pip install yfinance google-generativeai matplotlib pandas
