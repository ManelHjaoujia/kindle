# Kindle Review Sentiment Analysis

**Author:** Manel Hjaoujia  
**Project type:** Mini NLP Project — Sentiment Analysis 

---

## Project Overview

This project performs sentiment analysis on Kindle product reviews to classify review text into sentiment labels (e.g., positive / negative or rating-based classes).  
The notebook demonstrates a full NLP workflow: data loading, exploratory data analysis (EDA), preprocessing, feature extraction (TF-IDF and/or embeddings), model training and evaluation. 

---


## Notebook summary

The notebook contains the following key sections:

1. **Data loading & inspection**
   - Structure of dataset (columns: review text, rating, date, etc.)
   - Basic EDA: counts, missing values, distribution of ratings, sample reviews

2. **Preprocessing**
   - Text cleaning: lowercasing, punctuation removal, HTML/tag stripping (if any)
   - Tokenization, stopword removal (NLTK or spaCy), optional stemming/lemmatization
   - Handling class imbalance

3. **Feature engineering**
   - TF-IDF vectorization (with configurable `ngram_range`, `max_features`, `min_df`)
   - Optionally Word2Vec / FastText / pretrained embeddings for semantic features
   - Simple aggregated features: review length, number of exclamation marks, sentiment lexicon scores

4. **Modeling**
   - Classical ML model: Naive Bayes

5. **Evaluation**
   - Train/test split with stratification
   - Metrics: accuracy, precision, recall, F1 (per-class and macro), confusion matrix

---

### Quick interpretation
- TF-IDF + linear models are strong baselines for review sentiment due to frequent lexical cues.
- Tree-based or embedding-based models can capture non-linear interactions or semantic similarity, useful when phrasing varies.

---

## How to run / Reproduce

### 1. Clone repository
```bash
git clone https://github.com/ManelHjaoujia/kindle.git
cd kindle
```

### 2. Create environment & install dependencies

```bash
python -m venv venv
source venv/bin/activate        # macOS / Linux
venv\Scripts\activate           # Windows
pip install -r requirements.txt
```

## Key learnings:

* Built an end-to-end sentiment analysis pipeline for product reviews.

* Applied robust preprocessing, vectorization, and classic ML classifiers.

* Performed model evaluation with standard metrics and cross-validation.


### Author

**Manel Hjaoujia**

 Master’s Student — Information Systems Engineering & Data Science

 Passionate about NLP, Data Science, and machine learning applications





