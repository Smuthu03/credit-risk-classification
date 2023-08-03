# credit-risk-classification
Week 20 Credit Risk model
An overview of the analysis: Explain the purpose of this analysis.

The results: Using a bulleted list, describe the accuracy score, the precision score, and recall score of the machine learning model.

A summary: Summarize the results from the machine learning model. Include your justification for recommending the model for use by the company. If you don’t recommend the model, justify your reasoning.

# Module 20 Report Template

## Overview of the Analysis

* The purpose of the analysis is to create a model that could predict a good_loan ( a loan that is likly to be paid off in full without defalut) vs. a risky loan (where the borrower might fail to make the payment in its entirety).
* The credit Risk data included Loan_size, Interest_Rate, Borrower_income, debt_to_income, num_of_accounts, derogotory_marks, total_debt and loan_status for 77,536 loans. the goal is to create a model and understand how well the model can predict if the loan is a good_loan or risky_loan
* Goal was to predict the riskyness with regards to loan_status. the data included 75,036 good_loans and 2500 bad loans. 
* First I loaded the data and reviwed the data to understand the content of dataset.
* Then analyzed good and risky loan distribution with value_count function. then I separated the data into Labels and featurs (X and y) variable series
* Then I split the data using train_test_split with a random state of 1
* Then I created the logisitcRegression and fit the model with training data and then predited with training and test data
* Test dataset had 19,384 loans 


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1: LogisticRegression Model
  * Model score had 99.14% accuracy for the training set with a Recall score of 100%, precisition of 100% and f1Score of 100%
  * Model scored for the test set with 99.24% accuracy, 87% precistion, 89% recall score and 88% f1Score.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* The model seems to be predicting with really high precistion for good loan 100% of the time. however, it has ~12% to 13% false positive prediction.
* Predicting risky loan is critical as the company may experience higher loss if they do not optimize the model.  Though the model is fairly good I would recommend the company optimize the model towards prediticitng the false positive with higher accuracy to reduce the loss rate and balace the revenue from the loan account.

If you do not recommend any of the models, please justify your reasoning. I would recomment with causion in sing this model. Implement analyze, refine the model to minimize the loss
