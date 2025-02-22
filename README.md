# MACD Technical Analysis Tool

## Overview
This project implements a Moving Average Convergence Divergence (MACD) technical analysis tool for stock market analysis. MACD is a trend-following momentum indicator that shows the relationship between two moving averages of a security's price.

## Features
- Fetches real-time stock data using yfinance
- Calculates MACD indicator with customizable parameters:
  - Short-term EMA (default: 12 periods)
  - Long-term EMA (default: 26 periods)
  - Signal Line (default: 9 periods)
- Visualizes both stock price and MACD indicators
- Detects bullish and bearish crossover signals
- Interactive plots using matplotlib

## Technical Details
The tool calculates:
- MACD Line: Difference between short and long-term EMAs
- Signal Line: 9-day EMA of the MACD line
- MACD Histogram: Difference between MACD and Signal lines
- Crossover signals for potential trading opportunities

## Requirements
python
pandas
numpy
yfinance
matplotlib


## Installation
1. Clone this repository
2. Install required packages:
bash
pip install -r requirements.txt

## Usage
1. Open `macd_application.ipynb` in Jupyter Notebook
2. Modify the ticker symbol and date range as needed:
```python
ticker = 'NVDA'  # Change to any stock symbol
start_date = '2023-01-01'
end_date = '2025-02-21'
```
3. Run all cells to generate the analysis

## Output
The application provides:
- Numerical data showing MACD calculations
- Two-panel visualization:
  - Upper panel: Stock closing price
  - Lower panel: MACD line, Signal line, and Histogram

## License
MIT License