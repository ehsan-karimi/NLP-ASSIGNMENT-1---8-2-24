📌 Project Description: Wikipedia Text Classification (Geographic vs Non-Geographic)

This project classifies English Wikipedia articles as either geographic or non-geographic using Natural Language Processing (NLP) and machine learning. The pipeline was implemented using Python with the SpaCy and Scikit-learn libraries.

🔧 Pipeline & Operational Structure

Data Collection:
10 geographic and 10 non-geographic Wikipedia articles were selected as input.
Wikipedia articles were retrieved using the wikipedia Python package.
Text Preprocessing:
Texts were preprocessed using SpaCy (en_core_web_sm model):
Lowercased
Stop words removed (SpaCy’s list)
Lemmatization (via SpaCy)
Non-alphabetic tokens filtered out
Feature Extraction:
Transformed preprocessed texts into a Bag-of-Words representation using CountVectorizer.
Model Training:
Two classifiers were trained and evaluated:
Multinomial Naive Bayes
Logistic Regression (balanced class weights)
Evaluation:
Models were evaluated using a confusion matrix and classification report (precision, recall, F1-score).
Data was split into 70% training and 30% testing.
