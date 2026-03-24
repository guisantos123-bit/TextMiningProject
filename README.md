# Pokémon NLP Classification & Search Engine

This project combines Natural Language Processing (NLP), Machine Learning, and Web Scraping to build:

- A natural language search engine for Pokémon
- A text classification model that predicts Pokémon types from descriptions

---

## Key Results

- Logistic Regression: 82% accuracy  
- Naive Bayes: 81% accuracy  
- Random Forest: 76% accuracy  

Dataset:
- 1000+ Pokémon descriptions (web scraped from Bulbapedia)
- 800 Pokémon statistics
---

## Features

### Natural Language Search Engine
- Interprets user queries such as:
  - "fast, strong, fire type"
- Uses:
  - Fuzzy matching (Levenshtein distance)
  - Statistical filtering based on Pokémon attributes
- Returns:
  - Top 5 most relevant Pokémon ranked by similarity score

---

### Pokémon Type Predictor
- Predicts Pokémon type from text descriptions
- Pipeline includes:
  - Text preprocessing (tokenization, lemmatization)
  - TF-IDF vectorization
  - Supervised learning models:
    - Logistic Regression
    - Random Forest
    - Naive Bayes

---

## How It Works

1. Web scraping from Bulbapedia  
2. Text preprocessing (NLTK)  
3. TF-IDF vectorization  
4. Model training and evaluation  
5. Query processing with fuzzy matching  

---

## Tech Stack

- Python  
- NLP: NLTK  
- Machine Learning: Scikit-learn  
- Data Processing: Pandas, NumPy  
- Web Scraping: BeautifulSoup, Requests  
- Fuzzy Matching: RapidFuzz  

---

## Project Structure

TextMiningProject.ipynb # NLP + classification pipeline
PokemonSearcher.ipynb # Search engine implementation
data/ # Datasets (scraped + processed)

---

## Report

For a detailed explanation of methodology and results, see:
Relatório_TextMining_120090_120081.pdf

---

## Future Improvements

- Use advanced NLP models (Word2Vec, BERT, Transformers)  
- Deploy as a web application (Streamlit or Flask)  
- Improve semantic understanding of queries  

---

## Author

Guilherme Santos  
gmfts0609@gmail.com  
https://github.com/guisantos123-bit
