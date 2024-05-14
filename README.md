# Report
* All analysis code are located in the 'credit_risk_classification.ipynb' file
## Overview of the Analysis

* The purpose of this analysis is to predict whether a loan is high or low risk based on factors like loan size, interest rate, etc so we can ensure a stable economy.
* The financial information in this dataset are loan size, interest rate, borrower income, debt to income ratio, derogatory marks, number of accounts,and total debt to predict whether a loan is risky or not.
* We are prediciting "loan status" where 0 represents low risk and 1 represents high risk
* I first analyzed the data for any anomolies and created a training and testing data sets. We trained the model with the training data set and tested with the testing data, which is agnostic to the training data so it can be represent the model's performance as good as possible.
* In this analysis, we used logistic regression to predict whether a loan is risky. Logistic regression is commonly used for binary classifcation as it can provide us with a probability.

## Results

* Logistic Regression:
    * Accuracy: 99%. The model is able to correctly predict whether a sample is risky or low risk correctly 99% of the time.
    * Precision: 100%. When using lowrisk as true positive: of all the classifications that the model made that are low risk, 100% of them are actually low risk. When using high risk as a true positive: of all the classfication that are high risk, 85% of them are actually high risk.
    * Recall: 99%. When using lowrisk as true positive: of all the samples that are low risk, 99% of them are actually low risk. When using high risk as a true positive: of all the samples that are high risk, 91% of them are actually high risk.

## Summary

* The performance depend on the problem we are trying to solve. If the goal is to identify risky loans, it is more important to predict the '1', implying a high recall score is preferred. 
* It is recommended to use this model because the recall rate on predicting high risky loan is high. However, keep in mind the the class imbalance is high (18000: 600).


