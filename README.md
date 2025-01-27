# Fake News Detection Using Machine Learning

This project implements a fake news detection system using text preprocessing, feature extraction, and machine learning classification. It leverages logistic regression and decision tree classifiers to predict whether a news article is fake or real.

## Overview

- **Dataset**:
  - Two datasets are used: `Fake.csv` (fake news) and `True.csv` (real news).
  - Each dataset is labeled with a binary class: 0 for fake news, 1 for real news.
- **Data Preprocessing**:
  - Duplicates and unnecessary columns (`title`, `subject`, `date`) are removed.
  - Text is cleaned and standardized using regular expressions to remove noise (punctuation, numbers, URLs, etc.).
- **Feature Extraction**:
  - Text is vectorized using `TfidfVectorizer` to convert it into numerical features for classification.
- **Classification Models**:
  - Logistic Regression
  - Decision Tree Classifier
- **Evaluation**:
  - Both models are evaluated using metrics like accuracy and classification reports.
  - Manual testing allows for inputting custom news text to check predictions.

## Steps in the Code

1. **Dataset Loading**:
   - The `Fake.csv` and `True.csv` datasets are loaded into pandas DataFrames.
   - Labels are added to differentiate between fake and real news.
2. **Data Cleaning**:
   - Text preprocessing is performed using the `wordopt()` function to clean the data.
3. **Feature Engineering**:
   - TF-IDF vectorization is applied to convert the text data into numerical format.
4. **Model Training**:
   - Logistic Regression and Decision Tree models are trained on the processed dataset.
5. **Evaluation**:
   - Models are evaluated on test data, and their performance is printed using classification reports.
6. **Manual Testing**:
   - A custom function allows the user to input news text and view predictions from both models.

## Outputs

- Model accuracy scores for both Logistic Regression and Decision Tree classifiers.
- Classification reports displaying precision, recall, and F1-score.
- Predictions for user-input news using the manual testing function.

---

This project serves as a simple implementation of fake news detection using machine learning techniques.
