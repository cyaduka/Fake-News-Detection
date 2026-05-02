# Fake News Detection using NLP

This is a research paper project to detect fake news using a machine learning model trained on Kaggle's Fake and Real News dataset.

## Dataset
- Source: [Kaggle - Fake and Real News Dataset](https://www.kaggle.com/datasets/clmentbisaillon/fake-and-real-news-dataset)
- Two CSV files: `True.csv` (real news) and `Fake.csv` (fake news)
- Each file contains news articles with text and metadata

## Tech Stack
- Python
- Pandas, NumPy
- Scikit-learn
- TF-IDF Vectorizer
- PassiveAggressiveClassifier

## Approach
1. Combine `True.csv` and `Fake.csv` with labels (0 = REAL, 1 = FAKE)
2. Split into train and test sets
3. Convert news text into TF-IDF features
4. Train a PassiveAggressiveClassifier
5. Evaluate using accuracy, confusion matrix and classification report

## Results
| Metric | Score |
|--------|-------|
| Accuracy | ~92-93% |
| Precision | ~93% |
| Recall | ~93% |
| F1-Score | ~93% |

## How to Run

1. Clone the repository:
```
git clone https://github.com/cyaduka/Fake-News-Detection.git
cd Fake-News-Detection
```

2. Install dependencies:
```
pip install -r requirements.txt
```

3. Make sure `True.csv` and `Fake.csv` are in the project folder

4. Run the Jupyter notebook:
```
jupyter notebook Fake_News_Detection.ipynb
```

## Files
- `Fake_News_Detection.ipynb` - Main notebook (data loading, preprocessing, model, evaluation)
- `True.csv`, `Fake.csv` - Dataset files (download from Kaggle)
- `requirements.txt` - Python dependencies
- `README.md` - This file

## Author
- **Name:** Chirag Yaduka

