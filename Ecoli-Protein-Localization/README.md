# E. coli Protein Localization using Gaussian Naive Bayes

## Overview

A from-scratch implementation of Gaussian Naive Bayes and Quadratic Discriminant Analysis (QDA) for predicting protein localization sites using the E. coli dataset.

The project explores probabilistic classification, Gaussian distributions, covariance estimation, numerical stability, and model evaluation.

## Features

- Dataset inspection and preprocessing
- Selection of five protein localization classes: `cp`, `im`, `pp`, `imU`, and `om`
- Stratified 70/30 train-test split with a fixed random seed
- Gaussian Naive Bayes implementation from scratch
- Maximum Likelihood Estimation of class priors, means, and variances
- Variance floor analysis for numerical stability
- Log-probability calculations and Log-Sum-Exp normalization
- Confusion matrix, precision, recall, and F1-score evaluation
- Quadratic Discriminant Analysis using full covariance matrices
- Covariance regularization and model comparison

## Dataset

The project uses the E. coli protein localization dataset, containing 336 protein records, seven numerical features, and localization labels.

Only the following five classes are included:

- `cp`: Cytoplasm
- `im`: Inner membrane without signal sequence
- `pp`: Periplasm
- `imU`: Inner membrane, uncleavable signal sequence
- `om`: Outer membrane

The filtered dataset contains 327 records. Protein identifiers, when available, are excluded from the predictive features.

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

3. Place the E. coli dataset in the project directory.
4. Open the notebook:

   ```bash
   jupyter notebook ecoli_protein_localization.ipynb
   ```

5. Update the dataset file path if necessary and run the cells sequentially.

## Key Concepts

- Gaussian Naive Bayes
- Quadratic Discriminant Analysis (QDA)
- Maximum Likelihood Estimation
- Gaussian Probability Density
- Mean and Covariance Estimation
- Variance Floor
- Covariance Regularization
- Log Probabilities and Log-Sum-Exp
- Confusion Matrix
- Precision, Recall, and F1-Score
- Macro, Micro, and Weighted Averaging

## Evaluation

Both classifiers are evaluated on the same held-out test set.

The evaluation includes accuracy, confusion matrices, and per-class precision, recall, and F1-scores. Different variance floor values are also compared to investigate their effect on Gaussian Naive Bayes performance.

## Purpose

This project was developed as a practical machine learning exercise to understand and implement Gaussian probabilistic classifiers from scratch, with particular emphasis on their mathematical foundations, numerical stability, and performance evaluation.
