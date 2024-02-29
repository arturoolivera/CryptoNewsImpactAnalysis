# Introduction to GDeltCryptoNewsDownload Notebook

The purpose of this Jupyter notebook is to demonstrate the process of collecting and consolidating a dataset of news articles related to cryptocurrencies from the Global Database of Events, Language, and Tone (GDELT) project. This dataset, referred to as `GA_data.csv`, is intended for use in risk and fraud analysis projects where understanding the impact of news on the cryptocurrency market is crucial.

## Objective

To automate the retrieval of news articles from the GDELT database, focusing specifically on content related to various cryptocurrencies over a specified time period. This involves filtering articles by keywords associated with the cryptocurrency market, such as "cryptocurrency", "Bitcoin", "Ethereum", and others, to ensure the dataset is relevant to the project's needs.

## Methodology

The notebook utilizes the `gdeltdoc` Python library to interact with the GDELT database. This library simplifies the process of searching for and downloading news articles by providing a structured approach to specify search criteria (e.g., keywords, date ranges).

### Key Steps:

1. **Setting Up Filters**: Define a set of filters using the `Filters` class from the `gdeltdoc` library. These filters specify the keywords to search for (e.g., "crypto", "Bitcoin", "Ethereum", etc.) and the date range for the search. The date range is dynamically set to cover the period from the current day to the previous day to ensure the dataset is continually updated with the most recent news.

2. **Searching for Articles**: Execute a search query against the GDELT database using the defined filters. The search results are filtered to include only articles in English to maintain consistency in the dataset.

3. **Consolidating and Cleaning the Data**: The search results are compiled into a pandas DataFrame, with duplicates (based on article URLs) removed to ensure each article is unique. This step is repeated for each keyword and each day in the specified period, resulting in a comprehensive dataset of cryptocurrency-related news.

4. **Output**: The final DataFrame, containing unique news articles related to the specified keywords and within the given time frame, is saved to a CSV file named `GA_data.csv`. This file serves as the primary dataset for further analysis in the risk and fraud project.

## Usage

This notebook is designed to be executed on a regular basis (e.g., daily) to update the `GA_data.csv` file with the latest news articles. Users can modify the keyword list and the date range as needed to tailor the dataset to their specific project requirements.

## Requirements

- Python 3.x
- Pandas library
- GDELTDoc library (`gdeltdoc`)

## Conclusion

By leveraging the GDELT project's extensive database of global news articles, this notebook provides a streamlined process for collecting and preparing a dataset specifically focused on the cryptocurrency market. This dataset is invaluable for conducting risk and fraud analysis, offering insights into how news coverage can influence market behavior and potentially uncovering patterns or trends that could indicate fraudulent activities.
