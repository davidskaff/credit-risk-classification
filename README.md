# Loan Status Prediction Project

## Project Overview
This project involves building a machine learning model to predict loan status based on various financial indicators. The data contains financial information such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and total debt. The target variable is `loan_status`, which can be either a healthy loan (`0`) or a high-risk loan (`1`).

## Data
The data is stored in a CSV file located at "Resources/lending_data.csv". The CSV file contains the following columns: “loan_size”, “interest_rate”, “borrower_income”, “debt_to_income”, “num_of_accounts”, “derogatory_marks”, “total_debt”, “loan_status”.

## Machine Learning Process
The machine learning process involved several stages:
1. **Data Loading**: The data was loaded into a Pandas DataFrame from the CSV file.
2. **Data Review**: The DataFrame was reviewed to understand the data.
3. **Feature-Label Separation**: The data was separated into labels (`y`) and features (`X`).
4. **Data Splitting**: The data was split into training and testing sets using `train_test_split()`.
5. **Model Creation**: A Logistic Regression model was created.
6. **Model Fitting**: The model was fitted using the training data.
7. **Prediction**: Predictions were made on the testing data labels using the testing feature data (`X_test`) and the fitted model.

## Model Evaluation
The performance of the Logistic Regression model was evaluated using a confusion matrix and a classification report, which provided metrics such as precision, recall, and accuracy. The model performed well in predicting both healthy and high-risk loans, but there was room for improvement in predicting high-risk loans.

## Conclusion
While the Logistic Regression model is a good starting point, we might want to explore other models or techniques (like class balancing, different thresholds, etc.) to improve precision for high-risk loans (`1`) if that is deemed more important for the business scenario.
