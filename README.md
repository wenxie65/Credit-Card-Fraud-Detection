# Credit Card Fraud Detection

## Project Overview
This project focuses on credit card fraud detection using various machine-learning techniques. The goal is to build models that automatically categorize anonymized credit card transactions as fraudulent or genuine based on the patterns and anomalies in the dataset.

The dataset used for this project is the "Credit Card Fraud Detection" dataset from Kaggle, and it was collected and analyzed during a research collaboration between Worldline and the Machine Learning Group at the Université Libre de Bruxelles (MLG-ULB). The dataset contains transactions made by credit cards in September 2013 by European cardholders.

## Dataset Description
- The dataset contains 284,807 anonymized credit card transactions that occurred in two days and with 492 of them being frauds.
- Each row represents an individual credit card transaction, and each column represents different features derived from each transaction.
- The response variable 'Class' contains 1 in case of fraud and 0 otherwise.
- The dataset is available [here](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).

## Repository Contents
- `creditcard.csv`: The CSV file containing the credit card transaction records, with only the top 198000 rows due to the size.
- `fraud_detection.ipynb`: A Jupyter Notebook containing the Python code for the project.
