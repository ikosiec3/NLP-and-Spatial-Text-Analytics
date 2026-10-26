# Disneyland Reviews Sentiment Analysis

## Project Overview
This project analyzes visitor reviews from Disneyland locations in California, Hong Kong, and Paris. The primary goal is to investigate how the natural language used in reviews relates to star ratings (1–5) and to identify specific elements that visitors praise or complain about across different global locations.

## Data
The dataset contains over 42,000 reviews. Key features include:
*   Review text
*   Numerical rating (1-5 stars)
*   Reviewer location
*   Specific Disneyland branch

For the purpose of sentiment classification, ratings are categorized into three bins: 
*   **Negative:** 1-2 stars
*   **Neutral:** 3 stars
*   **Positive:** 4-5 stars

## Methodology
This project applies a comprehensive Natural Language Processing (NLP) pipeline to extract insights from unstructured text data.

### 1. Text Preprocessing
*   Tokenization and Lemmatization
*   Removal of punctuation and standard stopwords
*   Creation and application of domain-specific stopword lists to reduce noise
*   Feature extraction using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization

### 2. Sentiment Analysis Techniques
Multiple approaches were tested and compared to find the most effective method for this specific dataset:
*   **Dictionary-based methods:** VADER and SentiWordNet.
*   **Transformer-based models:** Utilizing BERT for advanced context understanding.
*   **Supervised Machine Learning:** Training models on TF-IDF features. Evaluated models include:
    *   Multinomial Naive Bayes
    *   Logistic Regression
    *   K-Nearest Neighbors (KNN)
    *   Random Forest
    *   Linear SVC
    *   XGBoost
*   **Optimization:** Applied hyperparameter tuning to maximize model performance.

## Results Summary
*   **Data Distribution:** The dataset is heavily imbalanced, with a strong dominance of positive reviews. 
*   **Location Insights:** Disneyland Paris exhibited the highest proportion of negative and neutral reviews among the three branches, highlighting potential areas for park-specific operational improvements.
*   **Model Performance:** Supervised Machine Learning models significantly outperformed traditional dictionary-based methods, particularly in correctly classifying the minority classes (negative and neutral reviews).
*   **Top Performers:** Logistic Regression and Linear SVC proved to be the most robust and effective models for this specific classification task.