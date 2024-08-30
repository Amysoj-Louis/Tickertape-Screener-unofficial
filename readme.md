# Tickertape-Screener-unofficial

This repository provides a Python script that queries the Tickertape API to fetch stock market data and presents it in a structured DataFrame format. The script extracts key information about stocks, including their names, tickers, sectors, market capitalization, and last traded prices.

## Overview

The script connects to the Tickertape API and retrieves data based on market capitalization. The data is processed and displayed in a DataFrame for easy viewing and analysis. The output includes the following columns:

- **Name**: The full name of the stock.
- **Ticker**: The stock's ticker symbol.
- **Sector**: The sector in which the stock operates.
- **Market Cap**: The market capitalization of the stock.
- **Last Price**: The last traded price of the stock.

## Features

- **API Integration**: Fetches data from the Tickertape API.
- **Data Processing**: Extracts and formats key stock information.
- **Data Display**: Presents data in a well-organized DataFrame format.

## Requirements

- **Python 3.7+**
- **Requests**: For making HTTP requests to the API.
- **Pandas**: For data manipulation and presentation.

## Installation

1. **Clone the repository**:


2. **Install the required packages**:

   It's recommended to use a virtual environment.

   ```bash
   pip install requests pandas
   ```

## Usage

1. **Run the script**:

   Make sure you have the necessary libraries installed, then execute the script using Python.

2. **View the output**:

   The script will fetch stock data from the Tickertape API, process it, and display it in a formatted DataFrame.

## Script Details

- **API URL**: `https://api.tickertape.in/screener/query`
- **Payload**: Configured to filter stocks by market capitalization and retrieve a set number of records.
- **Headers**: Include standard user-agent and accept headers for the API request.

## Example Output

The DataFrame produced by the script will look like:

| Name       | Ticker | Sector       | Market Cap | Last Price |
|------------|--------|--------------|------------|------------|
| Example Co | EXM    | Technology   | 1,000.00   | 150.00     |
| Sample Inc | SMP    | Finance      | 500.00     | 75.00      |

## Notes

- Ensure that the Tickertape API endpoint and parameters are up-to-date and valid.
- Adjust the API payload as needed to fit different data requirements.
