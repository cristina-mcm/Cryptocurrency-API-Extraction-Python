# Cryptocurrency API Extraction and Analysis

## Overview

This Python project retrieves cryptocurrency data from the CoinMarketCap API at timed intervals. Each observation is saved to a CSV file, which is then loaded into a pandas DataFrame for analysis. The collected data is used to visualize price trends, average percentage changes across different time periods, and the top and bottom five cryptocurrencies by 24-hour price change.

Data source: [CoinMarketCap API](https://coinmarketcap.com/api/)

The project:

1. Connects to the CoinMarketCap API using an API key.
2. Normalizes nested JSON responses into tabular data.
3. Adds a timestamp to each collection.
4. Creates a CSV file and appends new observations at timed intervals.
5. Loads the collected CSV data into a pandas DataFrame.
6. Groups and reshapes percentage-change data using pandas.
7. Visualizes average percentage changes across different time periods.
8. Plots Bitcoin prices over the collection period.
9. Uses the latest observation for each cryptocurrency to compare the top and bottom five 24-hour performers.

## Tools Used

- Python
- Requests
- pandas
- Seaborn
- Matplotlib
- Jupyter Notebook

## Repository Contents

- `Automating Crypto API Extraction.ipynb` – API extraction, data transformation, and visualizations
- `Crypto_API.csv` – Collected cryptocurrency data used for analysis
- `README.md` – Project documentation

## Notes

The collection loop operates only while the notebook and Python kernel remain running. Results represent the cryptocurrencies and observation period included in the dataset, not the entire cryptocurrency market.

## Acknowledgement

This was completed as a guided project based on Alex The Analyst’s Data Analyst Bootcamp tutorial, with updates for current pandas functionality and an additional analysis of the top and bottom 24-hour performers.
