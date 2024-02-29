# Introduction to Sentiment Analysis for Cryptocurrency News with FinBERT

In this Jupyter notebook, titled `ToReproduceSentiment.ipynb`, we embark on the journey of retraining the FinBERT model, a specialized transformer model for financial sentiment analysis, using the `CryptoLin_IE_v2.csv` dataset. The objective is to apply the retrained model for sentiment analysis on a dataset of cryptocurrency-related news articles. This process aims to enrich the dataset with sentiment scores, categorizing each news piece into positive, negative, or neutral sentiment. The enriched dataset, named `GA_data_wsentiment.csv`, will serve as an invaluable asset for deeper insights into the cryptocurrency market's reaction to news events.

## Objective

The primary goal is to leverage the FinBERT model, fine-tune it with cryptocurrency-specific news sentiment, and apply it to a pre-filtered dataset (`GA_data_wrelevance.csv`) of cryptocurrency news. This retraining and application process ensures that the sentiment analysis is attuned to the nuances of cryptocurrency discourse, thereby providing a more accurate and relevant assessment of news sentiment.

## Methodology

The approach encompasses several critical steps:

1. **Data Preparation and Cleaning**: Utilize the `CryptoLin_IE_v2.csv` dataset for training, which involves pre-processing steps such as text cleaning, stopwords removal, and lemmatization to prepare the data for the model.

2. **Model Retraining**: Fine-tune the FinBERT model with the prepared dataset to adapt its capabilities to the cryptocurrency news domain. This step involves setting up a training pipeline, defining metrics for evaluation, and executing the training process.

3. **Sentiment Analysis Deployment**: Apply the retrained model to the `GA_data_wrelevance.csv` dataset to perform sentiment analysis. Each news article is scored and classified into one of three sentiment categories: positive, negative, or neutral.

4. **Dataset Enrichment**: Append the sentiment scores and classifications to the dataset, resulting in `GA_data_wsentiment.csv`. This enriched dataset includes additional columns for sentiment probabilities and the final sentiment class for each news article.

5. **Output Generation**: The final dataset with appended sentiment analysis results is saved and ready for subsequent analysis phases, aiming to uncover insights into how news sentiment influences cryptocurrency markets.

## Usage

This notebook is a critical component of a larger analytical framework aimed at understanding the impact of news sentiment on the cryptocurrency market. By integrating sentiment analysis, stakeholders can gain nuanced insights into market sentiment, aiding in decision-making processes and market analysis.

## Requirements

- Python 3.x
- Pandas for data manipulation
- NumPy for numerical operations
- Transformers and PyTorch for model retraining and sentiment analysis
- NLTK for natural language processing tasks
- Scikit-learn for additional machine learning utilities

## Conclusion

The sentiment analysis performed in this notebook enhances our understanding of the cryptocurrency market's reaction to news events. By retraining the FinBERT model on cryptocurrency-specific news and deploying it on a relevant news dataset, we have created a valuable resource (`GA_data_wsentiment.csv`) for analyzing the market sentiment and its potential impacts on cryptocurrency prices and trends.
