# Credit Risk Analysis
## Overview
The purpose of Credit Risk Analysis is to mitigate the risks involved in lending money to individuals by establishing and utilizing a metric by which risk of loaning can be assessed. This can be determined by analysis of variables such as home ownership, last payment and much more through machine learning.

## Problem Statement
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. In this project, we will employ different techniques to train and evaluate models with unbalanced classes using imbalanced-learn and scikit-learn libraries.

## Methodology
We will be using the following techniques to train and evaluate the models:

- Oversample the data using the RandomOverSampler algorithms.
- Oversample the data using the SMOTE algorithms.
- Undersample the data using the ClusterCentroids algorithm.
- Use a combinatorial approach of oversampling and undersampling using the SMOTEENN algorithm.
- Compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results of Credit Risk Resampling Techniques

### Naive Random Oversampling
- Balanced Accuracy: 0.65%
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall High Risk: 62%
- Recall Low Risk: 68%

### SMOTE Oversampling
- Balanced Accuracy: 0.62%
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall High Risk: 59%
- Recall Low Risk: 66%

### Undersampling
- Balanced Accuracy: 0.51.6%
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall High Risk: 60%
- Recall Low Risk: 43%

### Combination (Over and Under) Sampling (using SMOTEENN Algorithm)
- Balanced Accuracy: 0.64.6%
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall High Risk: 71%
- Recall Low Risk: 58%

### Balanced Random Forest Classifier
- Balanced Accuracy: 0.78.7%
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall High Risk: 67%
- Recall Low Risk: 91%

### Easy Ensemble AdaBoost Classifier
- Balanced Accuracy: 0.92.5%
- Precision: The precision is low for High-risk loans and is high for Low-risk loans.
- Recall High Risk: 91%
- Recall Low Risk: 94%

Overall, the best model is the Easy Ensemble AdaBoost Classifier with a balanced accuracy score of 0.92.5%. However, it is important to note that the precision is low for high-risk loans in all models. Therefore, it is important to have human intervention to review all the high-risk results.

## Conclusion
In this project, we have employed different techniques to train and evaluate models with unbalanced classes using imbalanced-learn and scikit-learn libraries. The best model is the Easy Ensemble Classifier with a balanced accuracy score of 0.9316. It is important to have human intervention to review all the high risk results.
