# Fake News Detection using NLP
## Research Paper Project Report

**Author:** Chirag  
**Location:** Misraspatti, Uttarakhand, India  
**Date:** April 2026

---

## 1. Problem Statement

Fake news is spreading rapidly on social media platforms and news websites, causing misinformation among the public. The objective of this project is to use Natural Language Processing (NLP) techniques to automatically detect whether a news article is REAL or FAKE.

---

## 2. Dataset

| Detail | Value |
|--------|-------|
| Source | Kaggle Fake and Real News Dataset |
| Files | True.csv (real) + Fake.csv (fake) |
| Total Articles | 44,898 |
| Real News | 21,417 |
| Fake News | 23,481 |

---

## 3. Methodology

The project follows a 6-step NLP pipeline:

1. **Data Loading** - Combined True.csv and Fake.csv with labels (0=REAL, 1=FAKE)
2. **Preprocessing** - Removed unnecessary columns and used only the 'text' column
3. **TF-IDF Vectorization** - Converted text into numerical features
4. **Train-Test Split** - 80% training, 20% testing
5. **Model Training** - Trained PassiveAggressiveClassifier
6. **Evaluation** - Accuracy, Precision, Recall, F1-Score, Confusion Matrix

---

## 4. Results

### Accuracy: 99.51%

### Classification Report

| Class | Precision | Recall | F1-Score | Support |
|-------|-----------|--------|----------|--------|
| REAL (0) | 0.99 | 1.00 | 0.99 | 4,305 |
| FAKE (1) | 1.00 | 0.99 | 1.00 | 4,675 |
| Macro Avg | 1.00 | 1.00 | 1.00 | 8,980 |
| Weighted Avg | 1.00 | 1.00 | 1.00 | 8,980 |

### Confusion Matrix

| Actual \ Predicted | REAL | FAKE |
|---|---|---|
| REAL | 4,285 | 20 |
| FAKE | 24 | 4,651 |

---

## 5. Sample Predictions

| Input Text | Prediction |
|------------|------------|
| "US President Donald Trump inaugurated in 2025." | FAKE |
| "Aliens landed in Uttarakhand yesterday." | FAKE |

---

## 6. Conclusion

The NLP-based model using TF-IDF vectorization and PassiveAggressiveClassifier successfully detects fake news with **99.51% accuracy**. The model demonstrates excellent performance with near-perfect precision and recall for both REAL and FAKE news classes.

Future improvements can include using deep learning models such as LSTM or BERT for potentially better accuracy.

---

## 7. GitHub Repository

[https://github.com/cyaduka/Fake-News-Detection](https://github.com/cyaduka/Fake-News-Detection)

**Notebook:** Fake_News_Detection.ipynb (run on Google Colab)
**Dependencies:** Install using `pip install -r requirements.txt`
