# Stock Market Data Visualization

This Jupyter notebook demonstrates how to create interactive candlestick charts for stock market analysis using Python, yfinance, and Plotly.

## Code Structure

### 1. Data Collection
```python
import yfinance as yf
import plotly.graph_objects as go
from datetime import datetime, timedelta

# Define stock symbols and time period
symbols = ['AAPL', 'GOOGL', 'MSFT']
end_date = datetime.now()
start_date = end_date - timedelta(days=365)
```
This section sets up the required libraries and defines which stocks to analyze. The code fetches one year of historical data up to the current date.

### 2. Data Fetching
```python
data_dict = {}
for symbol in symbols:
    ticker = yf.Ticker(symbol)
    data_dict[symbol] = ticker.history(start=start_date, end=end_date)
```
The code uses yfinance to download historical stock data for each symbol and stores it in a dictionary. Each entry contains OHLC (Open, High, Low, Close) prices and volume data.

### 3. Visualization
```python
for symbol in symbols:
    data = data_dict[symbol]
    fig = go.Figure(data=[go.Candlestick(
        x=data.index,
        open=data['Open'],
        high=data['High'],
        low=data['Low'],
        close=data['Close']
    )])
    fig.update_layout(title=f'{symbol} Candlestick Chart',
                     xaxis_title='Date',
                     yaxis_title='Price')
    fig.show()
```
This section creates interactive candlestick charts using Plotly:
- Each candlestick represents one day of trading
- Green candlesticks indicate price increase (close > open)
- Red candlesticks indicate price decrease (close < open)
- The thin lines (wicks) show the high and low prices

## Features
- Interactive zooming and panning
- Hover tooltips showing price details
- One year of historical data
- Multiple stock comparison
- Professional-grade visualization

## Requirements
```bash
pip install pandas yfinance plotly nbformat ipython
```

## Usage
1. Open `Finance_data_visualization_v0.ipynb` in Jupyter Notebook/Lab
2. Run all cells sequentially
3. Interact with the charts:
   - Zoom: Click and drag on the chart
   - Pan: Click and drag the axes
   - Reset: Double click
   - Hover: Move mouse over candlesticks for details

## Data Source
Stock data is fetched in real-time from Yahoo Finance using the yfinance library, ensuring up-to-date market information.

## Author

Jin Lee
