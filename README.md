# Tweet Sentiment Classification

Binary sentiment classification model that categorizes tweets into **sadness** (`0`) and **happiness** (`1`) using classical NLP preprocessing and a Random Forest classifier.

## Overview
- **Dataset:** 10,374 labeled tweets (`5,209` happiness, `5,165` sadness)
- **Train/Test Split:** 80% training (`8,299` samples) / 20% testing (`2,075` samples) with `random_state=42`
- **Text Preprocessing:** Lowercasing, URL removal, punctuation/special character removal, digit removal, NLTK English stopword removal, and WordNet lemmatization
- **Feature Extraction:** Bag of Words (`CountVectorizer`, 13,741 features)
- **Model:** `RandomForestClassifier` (`n_estimators=100`, `random_state=42`)

## Evaluation Results
| Metric | Score |
| :--- | :--- |
| **Accuracy** | 76.19% (`0.7619`) |
| **Precision** | 77.57% (`0.7757`) |
| **Recall** | 72.22% (`0.7222`) |
| **AUC-ROC** | 83.67% (`0.8367`) |

## Repository Structure
- `tweet_sentiment_classification.ipynb` — Complete Jupyter notebook with data preparation, preprocessing, model training, and evaluation
- `tweet_sentiment_dataset.csv` — Input tweet dataset
- `README.md` — Project documentation
