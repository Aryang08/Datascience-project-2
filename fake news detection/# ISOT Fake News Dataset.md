# ISOT Fake News Dataset

## Overview
The **ISOT Fake News Dataset** contains two types of articles: fake news and real news. This dataset was collected from real-world sources, with truthful articles obtained by crawling content from [Reuters.com](https://www.reuters.com). The fake news articles were sourced from various unreliable websites flagged by Politifact (a fact-checking organization in the USA) and Wikipedia. The dataset encompasses different types of articles on various topics, although the majority focus on political and world news.

## Dataset Details
The dataset consists of two CSV files:{https://www.kaggle.com/datasets/emineyetm/fake-news-detection-datasets/data}
- **True.csv**: Contains over 12,600 articles sourced from Reuters.com.
- **Fake.csv**: Contains over 12,600 articles from various fake news outlets.

Each article includes the following information:
- **Title**: The title of the article.
- **Text**: The content of the article.
- **Type**: The classification of the article (fake or real).
- **Date**: The publication date of the article.

The dataset primarily focuses on articles published between 2016 and 2017. Although the collected data has been cleaned and processed, the original punctuation and errors in the fake news articles have been retained in the text for analysis.

## Methodology
This project involves the following steps:
1. **Data Loading**: Load the `True.csv` and `Fake.csv` files into Pandas DataFrames.
2. **Data Processing and Cleaning**: 
   - Remove unnecessary characters and whitespace.
   - Normalize the text (e.g., convert to lowercase).
   - Retain original punctuation and errors in fake news for analysis.
3. **Feature Extraction**: Convert the text data into numerical features suitable for machine learning classifiers (e.g., using TF-IDF or Count Vectorization).
4. **Model Training**: 
   - Utilize different classifiers to predict the veracity of news articles:
     - **Logistic Regression**
     - **Gradient Boosting**
     - **Random Forest**
5. **Model Evaluation**: Assess the performance of each classifier using appropriate metrics such as accuracy, precision, recall, and F1-score.

## Usage
1. Clone this repository or download the dataset.
2. Ensure you have the required libraries installed (e.g., `pandas`, `numpy`, `scikit-learn`).
3. Load the dataset using Pandas.
4. Perform data processing and cleaning.
5. Train the classifiers and evaluate their performance.

## Acknowledgements
- The dataset was collected from various reputable sources, including Reuters.com and fact-checking organizations.
- The classifiers used in this project are implemented using the Scikit-learn library.

## Requirements
To run this project, the following Python packages are required:
- pandas
- numpy
- scikit-learn
- (any additional libraries for text processing or visualization)
