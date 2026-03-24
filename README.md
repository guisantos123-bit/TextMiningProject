# TextMiningProject
Pokémon Classification Model and Search for Pokémons using Fuzzy Matching

## Abstract
This repository explores the intersection of Natural Language Processing (NLP), Web Scraping, and Search Algorithms within the Pokémon universe. It features a complete data science pipeline that extracts unstructured biological text data from the web, builds machine learning classification models, and implements a smart, fuzzy-matching search engine capable of understanding natural language queries.

## Key Features

### Web Scraping & Text Classification (TextMiningProject.ipynb)

-Data Extraction: Automated web scraping of over 1,000 Pokémon biology descriptions directly from Bulbapedia using BeautifulSoup.
-NLP Preprocessing: Comprehensive text cleaning including tokenization, stopword removal, and lemmatization using NLTK.
-Topic Modeling: Applied Non-Negative Matrix Factorization (NMF) alongside TF-IDF vectorization to discover latent biological themes (e.g., aquatic features, avian characteristics).
-Predictive Modeling: Trained and evaluated multiple Machine Learning classifiers (Logistic Regression, Random Forest, and Multinomial Naive Bayes) to predict a Pokémon's primary type strictly based on its text description.

### Pokemon Search (PokemonSearcher.ipynb)
-Natural Language Parsing: Processes user-inputted descriptions (e.g., "ataque alto, tipo fogo, rápido, pesado").
-Fuzzy Matching: Leverages Levenshtein distance (rapidfuzz) to correct typos and map informal user queries to exact Pokémon types and attributes.
-Dynamic Statistical Filtering: Translates qualitative terms (like "high" or "low") into quantitative DataFrame filters based on the 25th and 75th percentiles of base stats.
-Scoring System: Calculates a relevance score for each match based on the number of met criteria, returning an accurately sorted Top 5 list of Pokémon.

Language: Python
Data Collection: requests, BeautifulSoup4
Data Manipulation: pandas, numpy
NLP: nltk, unidecode
Machine Learning: scikit-learn
String Matching: rapidfuzz, python-Levenshtein
