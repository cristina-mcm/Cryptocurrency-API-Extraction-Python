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

## Key Findings

- The collected dataset contains 1,120 records representing 112 observations for 10 cryptocurrencies.
- Zcash showed the strongest longer-term performance among the cryptocurrencies analyzed, with increases of approximately 189% over 30 days and 211% over 90 days.
- Hyperliquid and Zcash were the strongest performers in the latest 24-hour observation, increasing by approximately 10.3% and 8.6%, respectively.
- Solana, BNB, and Ethereum also recorded positive 24-hour changes, while TRON was the only cryptocurrency in the latest observation with a notable decline.
- Tether and USDC remained close to zero across the measured periods, reflecting the comparatively stable behavior of USD-linked stablecoins.
- Bitcoin traded within a relatively narrow range during the short collection period, fluctuating between approximately $76,250 and $76,525.

## Visualizations

### Average Price Change by Time Period

<img width="610" height="491" alt="image" src="https://github.com/user-attachments/assets/49067162-002a-476e-bcb6-6421ac90acaa" />

This visualization compares average price changes over one hour, 24 hours, seven days, 30 days, 60 days, and 90 days.

### Top and Bottom 24-Hour Performers

<img width="983" height="580" alt="image" src="https://github.com/user-attachments/assets/5270ea21-7fc5-4a57-9472-00ebb22fe39e" />

This visualization uses the latest observation (September 17, 2026) for each cryptocurrency to compare the strongest and weakest 24-hour performers.

## Tools Used

- Python
- Requests
- pandas
- Seaborn
- Matplotlib
- Jupyter Notebook

## Repository Contents

- [Automating Crypto API Extraction.ipynb](Automating%20Crypto%20API%20Extraction.ipynb) — API extraction, data transformation, analysis, and visualizations
- [Crypto_API.csv](Crypto_API.csv) — collected cryptocurrency observations

## Notes

The collection loop operates only while the notebook and Python kernel remain running. Results represent the cryptocurrencies and observation period included in the dataset, not the entire cryptocurrency market.

## Acknowledgement

This was completed as a guided project based on Alex The Analyst’s Data Analyst Bootcamp tutorial, with updates for current pandas functionality and an additional analysis of the top and bottom 24-hour performers.
