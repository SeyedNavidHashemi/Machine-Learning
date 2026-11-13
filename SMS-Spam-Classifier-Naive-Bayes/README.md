# SMS Spam Classification using Naive Bayes

## Overview

A from-scratch implementation of a Multinomial Naive Bayes classifier for SMS spam detection using Python.

The project explores text preprocessing, feature extraction, probabilistic classification, model evaluation, and threshold optimization.

## Features

- Text preprocessing and tokenization
- Vocabulary construction with a minimum word-frequency threshold
- Multinomial Naive Bayes implementation from scratch
- Laplace smoothing and log-probability calculations
- Confusion matrix, precision, recall, and F1-score evaluation
- ROC curve and AUC calculation
- Neyman-Pearson threshold selection to maximize spam recall while keeping the false-positive rate (FPR) at or below 1%

## Dataset

The project uses the SMS Spam Collection dataset, containing labeled SMS messages classified as:

- `ham`: Legitimate messages
- `spam`: Unwanted or promotional messages

## Technologies

- Python
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

## How to Run

1. Clone the repository.
2. Install the required dependencies:

   ```bash
   pip install numpy pandas matplotlib jupyter
   ```

3. Open the notebook:

   ```bash
   jupyter notebook sms_spam_classifier.ipynb
   ```

4. Run the cells sequentially.

## Key Concepts

- Multinomial Naive Bayes
- Bag-of-Words representation
- Maximum Likelihood Estimation
- Laplace Smoothing
- Log probabilities
- ROC and AUC
- Neyman-Pearson classification

## Evaluation

The classifier is evaluated on a held-out test set. The Neyman-Pearson threshold is selected using the validation set to maximize spam recall under a specified FPR constraint.

## Purpose

This project was developed as a practical machine learning exercise to understand and implement a probabilistic text classification algorithm from scratch.
