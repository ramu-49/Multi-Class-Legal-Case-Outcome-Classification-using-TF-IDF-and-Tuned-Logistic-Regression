Multi-Class Legal Case Outcome Classification

📌 Project Overview

This project implements a multi-class legal text classification system to predict legal case outcomes (e.g., cited, applied, followed, referred to, affirmed, etc.) using classical NLP techniques. The model is built using TF-IDF feature extraction and tuned Multinomial Logistic Regression, with careful handling of class imbalance and performance evaluation.

📊 Dataset

Total Samples (after cleaning): 24,808

Train/Test Split: 80:20 (Stratified)

Target Classes: 10 legal outcome categories

Primary Feature: case_text

🔗 Data Source

Dataset sourced from Kaggle:
Legal Text Classification Dataset by A. Mohan Kumar
https://www.kaggle.com/datasets/amohankumar/legal-text-classification-dataset

🛠️ Methodology

Text preprocessing (lowercasing, stopword removal, punctuation & digit removal)

TF-IDF Vectorization (5,000 features, unigrams + bigrams)

Stratified 80:20 train-test split

Class imbalance handling (class_weight='balanced')

Hyperparameter tuning using GridSearchCV (Best C = 10)

📈 Final Performance

Accuracy: 44.9%

Weighted F1 Score: 0.47

Performance improved after tuning from 38% to 45% accuracy.
