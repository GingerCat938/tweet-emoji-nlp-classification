# Emoji Classification on Tweets – NLP Project

This repository contains one of my first university projects in Computational Linguistics using Python.

The project focuses on analyzing English tweets using Natural Language Processing [NLP] techniques and exploring the relationship between textual content and emoji labels.

It combines linguistic analysis (preprocessing, hashtags, Named Entity Recognition [NER], WordNet) with machine learning (sentence embeddings and MLP classification).

---

## Dataset

- Source: `cardiffnlp/tweet_eval`
- Task: Emoji classification
- Split used: validation (5,000 tweets)

Each tweet is associated with one of 20 emoji labels (0–19).

---

## Pipeline

The project follows these steps:

1. Data loading and preprocessing  
2. HTML cleaning and normalization  
3. Lemmatization and stopword removal (SpaCy + NLTK)  
4. Hashtag extraction and analysis  
5. Named Entity Recognition [NER]  
6. Sentence embeddings (SentenceTransformer)  
7. Classification with MLPClassifier  
8. Evaluation (classification report and confusion matrix)  
9. Semantic analysis with WordNet  

---

## Results

- Classification accuracy is below 50%, highlighting the difficulty of the task  
- Tweets are short, noisy, and highly variable  
- Semantic overlap between emoji classes makes prediction harder  

The confusion matrix shows a partially visible diagonal, but also significant dispersion across classes.

---

## Notebooks

- English version: `emoji_nlp_classification.ipynb`  
- Italian version: `emoji_nlp_classification_it.ipynb`  

The Italian notebook contains the original university version, while the English version is adapted for a broader audience.

---

## Installation

Install dependencies:

```bash
pip install -r requirements.txt

Download required resources:

python -m spacy download en_core_web_sm

Then in Python:

import nltk
nltk.download("stopwords")
nltk.download("wordnet")
Notes

This is an introductory academic project aimed at exploring the interaction between linguistic analysis and machine learning in NLP tasks.
