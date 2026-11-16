# Analyzing Historical Stock and Revenue Data: Tesla vs. GameStop

![Python](https://img.shields.io/badge/Python-3-3776AB?logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![yfinance](https://img.shields.io/badge/yfinance-stock%20data-green)
![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup-web%20scraping-orange)
![Plotly](https://img.shields.io/badge/Plotly-dashboards-3F4F75?logo=plotly&logoColor=white)

Final assignment for the IBM Python for Data Science course. The notebook builds a small pipeline that pulls **share-price history** from Yahoo Finance and **quarterly revenue** from web pages, then plots the two together for **Tesla (TSLA)** and **GameStop (GME)** so price movements can be compared against the business's actual revenue.

## What the notebook does

1. **Stock data:** download the full price history for each ticker with `yfinance`
2. **Revenue data:** download the revenue web page with `requests`, parse the HTML with `BeautifulSoup`, and extract the quarterly revenue table
3. **Cleaning:** strip `$` and `,` from revenue values and drop empty rows
4. **Visualization:** a two-panel Plotly dashboard per company (share price on top, revenue below), with data through June 2021

## Files

- `Final Assignment.ipynb`: the full notebook

## Running it

```bash
pip install yfinance beautifulsoup4 requests pandas plotly nbformat
jupyter notebook "Final Assignment.ipynb"
```

Needs an internet connection: stock data comes from Yahoo Finance and revenue pages from IBM's course site.

## Acknowledgements

Assignment template and data pages are from IBM / Coursera (IBM Skills Network).
