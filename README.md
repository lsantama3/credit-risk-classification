# credit-risk-classification

     The purpose of the analysis was to use varioius techniques to train and evaluate a model based on loan risk. The dataset that was used was on historical lending activity from peer-to-peer lending services company. This data was used in order to build a model that could identify the creditworthiness of borrowers.

The dependent variable that we focused on was loan_status. 0 for healthy loan and 1 for high-risk loans. The dataset had 75,036 data points for healthy loans and 2,500 data point for high-risk loans.
The independent variables were loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, and total_debt.

## Steps Taken
1. Read the lending_data.csv data from the Resources folder into a Pandas DataFrame.
2. Create the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.
3. Fit a logistic regression model by using the training data (X_train and y_train).
4. Save the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.
5. Evaluate the model’s performance by doing the following:
6. Generate a confusion matrix.
7. Print the classification report.
8. A second logisitc regression model was made but with RandomOverSampler.

### Logistic Regression Model 1:
- The model predicts with a 100% precision when it comes to healthy loans. When it comes to the high-risk loans it predicts it at a rate of 87%.
- Accuracy: 99%
- Recall: 94%

### Logistic Regression Model 2:
- The logisitic regression model predicts the healthy loans with a precision of 100% and and the high-risk loans at a precision of 87%.
- Accuracy: 100%
- Recall: 100%

## Summary
The best model to use woudl be Logistic Model 2. It predicted with the same amount of precison as the first model. However, if you compare the confusion matrixes you'll see fewer false predictions. It also has higher accuracy and recall
