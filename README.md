# WEEK-6-TASK
Advanced NLP — Named Entity Recognition, Topic Modeling & Transfer Learning

## Overview

This project demonstrates three advanced Natural Language Processing (NLP) techniques using the BBC News Dataset:

- Named Entity Recognition (NER)
- Topic Modeling (LDA)
- Text Classification using Transfer Learning (DistilBERT)

The project explores both traditional machine learning and modern transformer-based approaches for analyzing and classifying news articles.

---

## Dataset

**Name:** BBC News Dataset

**Source:** https://www.kaggle.com/datasets/jacopoferretti/bbc-articles-dataset

The dataset contains BBC news articles belonging to five categories:

- Business
- Entertainment
- Politics
- Sport
- Technology

---

# Project Structure

```
WEEK-6-TASK/
│
├── data/
│   └── BBC News Dataset
│
├── notebooks/
│   └── week6_advanced_nlp.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

# Part 1 – Named Entity Recognition (NER)

### Objectives

- Preprocess news articles
- Extract named entities using spaCy
- Identify the most frequent entity types
- Compare entity distribution across news categories
- Display example articles with extracted entities

### Techniques Used

- spaCy
- Entity Frequency Analysis
- Data Visualization (Matplotlib & Seaborn)

---

# Part 2 – Topic Modeling

### Objectives

- Preprocess text
- Apply Latent Dirichlet Allocation (LDA)
- Discover hidden topics
- Assign dominant topics to articles
- Compare discovered topics with actual news categories
- Evaluate topic quality using Coherence Score

### Techniques Used

- Gensim
- LDA (Latent Dirichlet Allocation)
- Coherence Score (C_V)

---

# Part 3 – Text Classification

Two different approaches were implemented.

## Baseline Model

- TF-IDF Vectorization
- Logistic Regression

### Accuracy

**98.12%**

---

## Transfer Learning

Pre-trained Model:

**DistilBERT**

The model was fine-tuned on the BBC News Dataset for multi-class news classification.

### Accuracy

**98.36%**

---

# Model Comparison

| Model | Accuracy |
|--------|----------|
| Logistic Regression | 98.12% |
| DistilBERT | 98.36% |

DistilBERT achieved the highest overall performance while leveraging pre-trained language representations.

---

# Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- spaCy
- NLTK
- Gensim
- Scikit-learn
- Hugging Face Transformers
- Hugging Face Datasets
- PyTorch

---

# Results

### Named Entity Recognition

- Extracted people, organizations, locations, and geopolitical entities.
- Compared entity frequencies across different news categories.

### Topic Modeling

- Discovered latent topics using LDA.
- Achieved a Coherence Score of **0.5227**.

### Text Classification

Successfully compared:

- Traditional Machine Learning
- Transfer Learning

DistilBERT slightly outperformed Logistic Regression while both models achieved excellent classification accuracy.

---

# Future Improvements

- Interactive topic visualization using pyLDAvis
- Hyperparameter tuning for LDA
- Experiment with larger transformer models (BERT, RoBERTa)
- Deploy the fine-tuned model using Streamlit or FastAPI

---

# Author

**Hania Sajjad**

AL/ML Intern
ITSimplera Solutions
