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
- `creditcard.csv`: The CSV file containing the credit card transaction records, with only the top 198000 rows due to the file size limit. Used for training and evaluation.
- `fraud_detection.ipynb`: A Jupyter Notebook containing the Python code for the project.

## Machine Learning Techniques
This project utilizes the following machine learning techniques:
1. Logistic Regression
2. Decision Trees
3. Random Forest

## Dependencies
To run the project, ensure that the required Python packages are installed 
 - pandas
 - numpy
 - matplotlib
 - scikit-learn (sklearn)

To install these packages using pip, open a terminal or command prompt and run the following command:
```shell
pip install pandas numpy matplotlib scikit-learn
```

## Installation
1. Clone Credit-Card-Fraud-Detection repository to local machine:
```shell
git clone https://github.com/wenxie65/Credit-Card-Fraud-Detection.git
```
2. Navigate to the project directory:
```shell
cd Credit-Card-Fraud-Detection
```
3. Run `fraud_detection.ipynb`:
```shell
python fraud_detection.ipynb
```

## Results
The results of this project can be found in the [results.md](results.md) file. It provides the performance report for each model and helps identify the most effective technique for credit card fraud detection.

To view the results, please refer to the [results.md](results.md) file.
