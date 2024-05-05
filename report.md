# Module 12 Report Template

## Overview of the Analysis

The purpose of the analysis was to build a machine learning model to predict loan status, which can be either a healthy loan (`0`) or a high-risk loan (`1`), based on various financial indicators. The data contained financial information such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The target variable was `loan_status`, and the features included all other variables. The machine learning process involved several stages: data loading, data review, feature-label separation, data splitting into training and testing sets, model creation, model fitting, and prediction. The model used was Logistic Regression, a common algorithm for binary classification problems. The model's performance was evaluated using a confusion matrix and a classification report, which provided metrics such as precision, recall, and accuracy. The model performed well in predicting both healthy and high-risk loans, but there was room for improvement in predicting high-risk loans. This analysis is crucial in the financial sector as it helps in risk assessment and decision-making related to loan approval.

## Results

Accuracy: The model had an accuracy of 0.99, meaning it correctly predicted the loan status for 99% of all loans in the test set.
Precision: For the healthy loan (0) label, the precision was 1.00, meaning all loans that the model predicted as healthy were indeed healthy. For the high-risk loan (1) label, the precision was 0.85, meaning 85% of the loans that the model predicted as high-risk were indeed high-risk.
Recall: For the healthy loan (0) label, the recall was 0.99, indicating that the model was able to correctly identify 99% of all actual healthy loans. For the high-risk loan (1) label, the recall was 0.91, indicating that the model was able to correctly identify 91% of all actual high-risk loans.

## Summary

The Logistic Regression model used in this analysis performed quite well, with an overall accuracy of 0.99. It was excellent at predicting healthy loans (`0`), with a precision and recall of 1.00 and 0.99, respectively. However, it was slightly less precise (0.85) but still good at recall (0.91) for high-risk loans (`1`). The performance of a model does indeed depend on the problem we are trying to solve. In this case, if the cost of misclassifying a high-risk loan as healthy is high (which is usually the case in lending scenarios), we might want a model that is better at predicting `1`s, even if it comes at the cost of misclassifying some `0`s. Therefore, while the Logistic Regression model is a good starting point, we might want to explore other models or techniques (like class balancing, different thresholds, etc.) to improve precision for high-risk loans (`1`) if that is deemed more important for the business scenario.
