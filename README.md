# 📩 SMS Spam Classifier — Naive Bayes

> A learning-focused NLP project that classifies SMS messages as **Ham** or **Spam** using **Multinomial Naive Bayes**, **TF-IDF**, **Bigrams**, and **Handcrafted Features**.

---

## 🚀 Overview

This project implements an SMS spam classifier using the classic SMS Spam dataset.

Instead of building a basic:

`CountVectorizer → MultinomialNB → Accuracy`

pipeline, this project explores a more complete machine-learning workflow involving:

- 🧹 Text preprocessing
- 🔢 TF-IDF feature extraction
- 🔗 Unigrams + Bigrams
- 🛠️ Handcrafted text features
- ⚡ Sparse feature matrices
- 🎯 Hyperparameter tuning with `GridSearchCV`
- 🔄 5-Fold Cross Validation
- 📊 Precision, Recall & F1-score
- 🧩 Confusion Matrix
- 📈 ROC-AUC & ROC Curve

The main goal is to understand **why each step matters**, rather than simply training a model.

---

## 🎯 Objective

Classify an SMS message into one of two classes:

| Label | Meaning |
|------|---------|
| `ham` | Normal / legitimate SMS |
| `spam` | Spam SMS |

The labels are encoded as:

```text
ham  → 0
spam → 1
