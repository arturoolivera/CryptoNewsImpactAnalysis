# Cryptocurrency News Impact Analysis

## Project Overview

This repository contains a series of Jupyter notebooks dedicated to analyzing the impact of news on the cryptocurrency market. Utilizing data from the Global Database of Events, Language, and Tone (GDELT) project, this analysis spans various aspects such as relevance, sentiment, strength of news items, and their overall impact on cryptocurrency fluctuations. The project aims to provide insights into how news influences market behavior, aiding in risk and fraud analysis, investment strategies, and market understanding.

## Definitions

### Relevance

**Relevance** in the context of this project refers to the degree to which a news article pertains to the cryptocurrency market. A high relevance score indicates that the article provides significant information related to cryptocurrencies, which could include market trends, regulatory changes, technological advancements, or other news impacting the cryptocurrency ecosystem. Relevance scores help filter out unrelated news, ensuring that the analysis focuses on content that can influence cryptocurrency markets.

### Sentiment

**Sentiment** analysis measures the tone and emotional context of a news article. It categorizes the sentiment of cryptocurrency-related news into positive, negative, or neutral. This classification helps in understanding the general mood or attitude conveyed by the news article towards the subject matter. Sentiment scores are crucial for assessing how news might affect investor perception and market trends, providing insights into potential market movements based on the nature of the news coverage.

### Strength

**Strength** refers to the potential impact or influence a news article has on the cryptocurrency market's behavior. It takes into account factors such as the article's relevance, sentiment, and the specific details contained within the text to assess how strongly the news might affect market prices, volatility, or investor sentiment. Strength scores aim to quantify the financial significance of news items, identifying those with the power to move markets or signal significant changes in the cryptocurrency landscape.

## Models Explanations

### FinBERT

**FinBERT** is a variant of the BERT (Bidirectional Encoder Representations from Transformers) model, specifically fine-tuned for financial sentiment analysis. Developed by leveraging the pre-trained BERT model, FinBERT is adapted to the nuances of financial language through training on a dataset of financial news and information. This specialization allows FinBERT to accurately categorize financial texts into positive, negative, or neutral sentiments, making it an invaluable tool for analyzing the sentiment of news articles related to the cryptocurrency market. By applying FinBERT, this project can assess how news sentiment might influence investor behavior and market trends, providing deeper insights into the potential impact of news on the cryptocurrency ecosystem.

### GDELT

**GDELT (Global Database of Events, Language, and Tone)** is an open-source platform that monitors the world's broadcast, print, and web news from nearly every corner of every country in over 100 languages and identifies the people, locations, organizations, themes, sources, emotions, counts, quotes, images, and events driving our global society every second of every day. This vast collection of data enables comprehensive analysis of the global news landscape, including the ability to track the spread of information and how it influences public perception and behavior. In the context of this project, GDELT is utilized to automate the retrieval of news articles related to cryptocurrencies, providing a rich dataset for relevance, sentiment, and strength analysis.

### Fama French Model

The **Fama French Model** is a widely recognized asset pricing model that expands on the Capital Asset Pricing Model (CAPM) by adding size and value factors to the market risk factor in CAPM. This model is based on three factors: (1) market risk, (2) the outperformance of small-cap stocks compared to large-cap stocks, and (3) the outperformance of high book-to-market value stocks over low book-to-market value stocks. In financial analysis, the Fama French model is used to explain why certain stocks are priced differently from others and to predict future returns based on these three factors. For this project, the Fama French model is employed to assess the financial strength of news items, evaluating their potential impact on the cryptocurrency market by analyzing correlations between news content, market returns, and the three Fama French factors.


## Repository Structure

- **Data_Ingestion_GA.ipynb**: Automates the retrieval of news articles related to cryptocurrencies from GDELT, generating a dataset for further analysis.
- **Relevance_Analysis_GA.ipynb**: Trains a machine learning model to score the relevance of news articles, enhancing the dataset with relevance scores.
- **Sentiment_Analysis_GA.ipynb**: Applies the FinBERT model to assess the sentiment of cryptocurrency-related news, appending sentiment scores to the dataset.
- **Strength_Analysis_GA.ipynb**: Utilizes the Fama French model to evaluate the financial strength of news items, further enriching the dataset.
- **EDA_Cryptocurrency_News_Impact.ipynb**: Conducts exploratory data analysis on the enriched dataset to uncover insights into the impact of news on the cryptocurrency market.

## Prerequisites

- Python 3.x
- Libraries: Pandas, NumPy, Matplotlib, Seaborn, NLTK, Scikit-learn, PyTorch, Transformers, Statsmodels
- Data: GDELT for initial data retrieval, various datasets for model training and analysis

Ensure you have Python installed and can run Jupyter notebooks. Clone this repository to your local machine to get started.

## Installation

1. Clone the repository to your local environment.
2. Install required Python packages using:
   ```bash
   pip install -r requirements.txt
3. The first notebook (`Data_Ingestion_GA.ipynb`) includes a command to automatically download and install the dependencies listed in `requirements.txt`.

## Usage

To replicate the analysis or apply the methodology to new datasets, follow these steps:

1. **Data Collection**: Run `Data_Ingestion_GA.ipynb` to collect the latest cryptocurrency news data from GDELT.
2. **Model Training and Application**:
- Execute `Relevance_Analysis_GA.ipynb` to score news relevance.
- Run `Sentiment_Analysis_GA.ipynb` to perform sentiment analysis.
- Follow with `Strength_Analysis_GA.ipynb` to evaluate news strength.
3. **Exploratory Data Analysis**: Analyze the enriched dataset with `EDA_Cryptocurrency_News_Impact.ipynb` for insights into news impact.

Each notebook is self-contained with detailed instructions and explanations, making it easy to follow or adapt to your specific needs.

## Contributing

Contributions to improve the analysis or extend the project are welcome. Please open an issue or submit a pull request with your suggestions or enhancements.

## Acknowledgments

- The GDELT Project for providing access to a vast repository of global news data.
- OpenAI and contributors for the development of advanced machine learning models and libraries used in this analysis.

## Contact

For any queries or further discussion, feel free to open an issue in this repository.

