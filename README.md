# SQL Injection Detection with Logistic Regression

## Overview
This project implements a **Logistic Regression** machine learning model to detect potential SQL Injection attacks in user inputs.  
The model is trained on labeled data containing examples of benign and malicious SQL queries, enabling it to classify incoming requests as **safe** or **suspicious**.

## Features
- **Binary classification**: Distinguishes between normal and malicious SQL input.
- **Text preprocessing**: Tokenization, lowercasing, and removal of special characters.
- **Feature extraction**: Uses TF-IDF vectorization to represent input text numerically.
- **Logistic Regression model**: Selected for its simplicity, interpretability, and strong performance on text classification tasks.

## Dataset
- The dataset consists of:
  - **Benign queries** (legitimate SQL statements or harmless user input)
  - **Malicious queries** (containing common SQL Injection payloads)
- Preprocessed to remove duplicates, normalize text, and split into training/testing sets.

## Model Training
1. **Data preprocessing**:
   - Lowercasing and cleaning special characters
   - Tokenization
   - TF-IDF vectorization
2. **Model fitting**:
   - Logistic Regression classifier trained on processed features
3. **Evaluation**:
   - Metrics: Accuracy, Precision, Recall, F1-score
   - Confusion matrix for detailed performance analysis
