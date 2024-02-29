# Model Training for Score Relevance

## Project Overview

This notebook is part of a series dedicated to building a relevance score model. The goal is to differentiate relevant news articles from two distinct sources:
- Target 1: News from [Yahoo Finance on Crypto](https://finance.yahoo.com/topic/crypto) 
- Target 0: General news from [Yahoo News](https://news.yahoo.com)

The model employs a pipeline combining `TfidfVectorizer` and `MultinomialNB` (Naive Bayes) for classification.

## Notebook Objective

`Relevance_Analysis_GA.ipynb` focuses on training a supervised relevance score model using the `all_score_training.csv` dataset. This model is then applied to classify news articles downloaded from Gdelt in an additive manner.

- **Development Dataset**: `all_score_training.csv`
- **Deployment Dataset**: 
    - **Input**: `GA_data.csv`
    - **Output**: `GA_data_wrelevance.csv`

## Model Training Approach

The training involves several key steps:
1. **Data Preprocessing**: Utilizing custom transformers for text cleaning, stop words removal, and lemmatization.
2. **Feature Extraction**: Applying `TfidfVectorizer` to convert text data into a format suitable for model training.
3. **Model Training**: Employing `MultinomialNB` within a pipeline for classification.
4. **Evaluation**: Assessing the model's performance using metrics such as accuracy, precision, recall, F1 score, and ROC AUC.

## Implementation Details

The process begins with essential imports and data loading. Custom transformers (`TextCleaner`, `StopWordsRemover`, `Lemmatizer`) are defined for data preprocessing, followed by the establishment of a pipeline integrating these transformers with `TfidfVectorizer` and `MultinomialNB`.

The dataset `all_score_training.csv` is used for training, with the target variable indicating the relevance of news articles (1 for relevant, 0 for non-relevant). The pipeline is trained and evaluated on this dataset, and performance metrics are reported.

Finally, the trained model is saved for future use in classifying new datasets, demonstrated by applying it to `GA_data.csv` and producing `GA_data_wrelevance.csv`.

## Conclusion

This notebook showcases the end-to-end process of building a relevance score model, from preprocessing and feature extraction to training, evaluation, and deployment. The approach is designed to be reproducible and scalable, allowing for efficient classification of news articles based on their relevance to specific topics.
