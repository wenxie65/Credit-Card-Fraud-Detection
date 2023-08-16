# Credit Card Fraud Detection

## Project Overview
This project focuses on credit card fraud detection using various machine-learning techniques. The goal is to build models that automatically categorize anonymized credit card transactions as fraudulent or genuine based on patterns and anomalies in the dataset.

The dataset used for this project is the 'Credit Card Fraud Detection' dataset from Kaggle, collected and analyzed during a research collaboration between Worldline and the Machine Learning Group at the Université Libre de Bruxelles (MLG-ULB). The dataset comprises transactions made by credit cards in September 2013, involving European cardholders.

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
2. Decision Tree
3. Random Forest

## Logistic Regression
The Logistic Regression model achieved an AUPRC score of 0.9316, indicating its ability to effectively prioritize fraudulent transactions with higher predicted probabilities. Moreover, the feature coefficients of the model provided insights into how different principal components influenced the prediction outcomes.

## Decision Tree
The initial Decision Tree model yielded an AUPRC score of 0.8499. As several features were assigned zero importance by the model, a Decision Tree model was constructed solely using features with non-zero importance. Surprisingly, this resulted in a lower AUPRC score of 0.5513, suggesting that incorporating the entire feature set resulted in improved model performance.

## Random Forest
The Random Forest model delivered an AUPRC score of 0.9316, which is equivalent to the performance of the Logistic Regression model. The analysis of feature importances within the Random Forest model shows that these importances were distributed across diverse principal components.

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

## Model Comparison and Insights
Comparing the three models, both the Logistic Regression and Random Forest models delivered equal AUPRC scores of 0.9316. Despite the Decision Tree model offering interpretability, it displayed decreased performance compared to the other two models. This reduced performance may be resulted by its limited capacity to capture complex relationships among features.

## Conclusion
This project involved a comprehensive analysis of fraud detection using machine learning techniques, including the evaluation of the capabilities of Logistic Regression, Decision Trees, and Random Forests. The AUPRC scores of the Logistic Regression and Random Forest models highlight their suitability for detecting fraudulent transactions. The feature importance analyses offer insights into the factors impacting fraud detection.

As this project concludes, it is important to acknowledge the potential for improvements. Further explorations, such as hyperparameter tuning and additional feature engineering, have the potential to enhance the performance of the models even further.
