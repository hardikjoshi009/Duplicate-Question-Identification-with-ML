# Duplicate Question Identification with ML

This project develops a machine learning model to identify duplicate or similar question pairs on Quora. The goal is to automatically detect questions that are semantically similar, aiding in efficiently linking new questions to existing answers.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Feature Engineering](#feature-engineering)
- [Models Used](#models-used)
- [Results](#results)

## Overview

The project focuses on detecting pairs of similar questions from Quora using machine learning. Through feature engineering, we extract meaningful insights from the question text, which are then used to train machine learning models. The solution links new or duplicate questions to pre-existing answers, reducing redundancy on platforms like Quora.

## Features

- **Feature Engineering**: Extracts critical features such as word overlap, cosine similarity, Levenshtein distance, and more.
- **Machine Learning Models**: Uses three models—Linear Logistic Regression, SVM, and XGBoost.
- **Evaluation**: Tracks model performance using accuracy metrics on labeled question pairs.

## Feature Engineering

Feature engineering is crucial for determining the similarity between question pairs. This project involves:

- **Word overlap**: Measures the number of common words between two questions.
- **Cosine similarity**: Evaluates the cosine of the angle between question vectors.
- **Levenshtein distance**: Calculates the edit distance between two strings.
- **TF-IDF and Word Embeddings**: Represents questions using Term Frequency-Inverse Document Frequency and word embeddings to capture semantic similarity.

## Models Used

Three machine learning models were used for training:

1. **Linear Logistic Regression**:
   - A basic linear model that fits the engineered features to determine if two questions are duplicates.
   - Achieved an accuracy of **70.36%**.
   
2. **Support Vector Machine (SVM)**:
   - A more complex model that separates similar and dissimilar question pairs using hyperplanes.
   - Achieved an accuracy of **75.8%**.

3. **XGBoost**:
   - A gradient boosting model that combines the outputs of weak learners to form a strong prediction model.
   - Achieved the best performance with an accuracy of **78%**.

## Results

The following are the accuracy scores achieved with different models on the Quora duplicate question dataset:

- **Linear Logistic Regression**: 70.36%
- **Support Vector Machine (SVM)**: 75.8%
- **XGBoost**: 78%

---

This README provides an overview of the problem, explains the key steps in feature engineering, and presents the results of the models used.