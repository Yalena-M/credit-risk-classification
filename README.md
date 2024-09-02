# credit-risk-classification# Module 12 Report Template

## Overview of the Analysis

The analysis aimed to evaluate the effectiveness of machine learning models in predicting loan risk, specifically identifying healthy loans versus high-risk loans. The dataset contained historical lending activity with the target variable, loan_status, indicating whether a loan was healthy (0) or high-risk (1). The analysis required predicting this binary outcome based on various financial features.

## Results

Machine Learning Model 1:
Data Preparation: Loaded the data, Separated the target variable from the features, and split the dataset into training and test sets.
Model Training: Fit a logistic regression model to the training data.
Model Evaluation: Assess model performance using metrics such as accuracy, precision, recall, and F1-score.
confusion matrix:
18658 = True Negatives (TN)
107 = False Positives (FP)
37 = False Negatives (FN)
582 = True Positives (TP)

classification report:
Accuracy: 0.99
Precision for healthy loans (0): 1.00
Recall for healthy loans (0): 0.99
F1-score for healthy loans (0): 1.00
Precision for high-risk loans (1): 0.84
Recall for high-risk loans (1): 0.94
F1-score for high-risk loans (1): 0.89

## Summary

The logistic regression model performs exceptionally well, with an overall accuracy of 99%. It shows perfect precision a high recall for predicting healthy loans, and strong performance for high-risk loans with a recall of 94% and an F1-score of 0.89. we compare their metrics on key performance indicators such as accuracy, precision, and recall.   SVM demonstrates higher precision for predicting high-risk loans. This precision is crucial in financial settings where accurately identifying high-risk loans is vital to minimizing false positives and potential losses. Although the Logistic Regression model has a slightly higher overall accuracy, the SVM model demonstrates superior precision in predicting high-risk loans. This higher precision is crucial because even a model with 100% true positives can still have false positives, which SVM minimizes more effectively. Therefore, precision for high-risk loans is highly valued. SVM’s higher precision means it is more effective at avoiding false positives in high-risk loan predictions, which is critical for reducing unnecessary scrutiny or actions for loans that are not truly high-risk. If minimizing false positives for high-risk loans is the priority, SVM's higher precision makes it preferable. If identifying as many high-risk loans as possible is the priority, despite potential false positives, Logistic Regression's higher recall may be preferable.
