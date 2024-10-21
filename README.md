# credit-risk-classification

## Overview of the Analysis
The goal of this challenge was to train and evaluate a model based on loan risk. We begin by calling the data from the loan_data.csv file. After, we used a Logisitic regression to predict loan_status using the other feautures in the file: loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, and total_debt. We do this by splitting the data, initializing the model, and pluggin the variables into a confusion matrix and classification report.

## Results
* Logisitic Regression:
    * Accuracy: 0.99 
      * this implies that 99% of the predictions were correct
    * Precision:
      * Healthy Loan (0): 1.00
        * Statistically perfect at predicting healthy loans
      * High-Risk Loan (1): 0.84
        * 84% of loans predicted to be high-risk were high risk
    * Recall:
      * Healthy Loan (0): 0.99
        * 99% of healthy loans were correctly identified
      * High-Risk Loan (1): 0.94
        * 94% of high-risk loans were correctly identified

## Summary
This logisitic model performs very well. With an overall accuracy of 0.99, the model is very reliable when predicting healthy loans. If the goal was only to predict healthy loans, this model is perfect, but if more accuracy is desired when predicting risky loans, a different model may be useful. Changing hyperparameters may also help.