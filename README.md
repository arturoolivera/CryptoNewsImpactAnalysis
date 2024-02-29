# Cryptocurrency News Impact Analysis

## Project Overview

This repository contains a series of Jupyter notebooks dedicated to analyzing the impact of news on the cryptocurrency market. Utilizing data from the Global Database of Events, Language, and Tone (GDELT) project, this analysis spans various aspects such as relevance, sentiment, strength of news items, and their overall impact on cryptocurrency fluctuations. The project aims to provide insights into how news influences market behavior, aiding in risk and fraud analysis, investment strategies, and market understanding.

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

## License

This project is open-sourced under the MIT License. See the LICENSE file for more details.

## Acknowledgments

- The GDELT Project for providing access to a vast repository of global news data.
- OpenAI and contributors for the development of advanced machine learning models and libraries used in this analysis.

## Contact

For any queries or further discussion, feel free to contact the project maintainers or open an issue in this repository.

