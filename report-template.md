# Module 12 Report Template

## Overview of the Analysis

* In this anaylsis I have used a Logistic Regression to evaluate a model based on loan risk. 
* The data used for this model is historical lending activity from a peer-to-peer lending service.
* The dataset contains the following columns `	loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, total_debt, loan_status`. 
* I will use this data to predict the creditworthiness of borrowers.
* The dataset was seperated into labels and features and then split into training and testing using `train_test_split.`
* To predict the creditworthiness of borrowers a `LogisticRegression` was used.

## Results


* Machine Learning Model 1:
    * Class 0 (healthy loan):

    * Precision: 1.00 (the model is perfect in predicting healthy loans)
    * Recall: 0.99 (the model correctly identifies 99% of actual healthy loans)
    * F1-score: 1.00 (the harmonic mean of precision and recall is perfect)
    * Support: 18,765 (the number of actual healthy loan instances)
    
    * Class 1 (high-risk loan):

    * Precision: 0.85 (the model correctly predicts 85% of high-risk loans)
    * Recall: 0.91 (the model correctly identifies 91% of actual high-risk loans)
    * F1-score: 0.88 (the harmonic mean of precision and recall)
    * Support: 619 (the number of actual high-risk loan instances)
    * Overall Accuracy: 0.99 (the model's overall accuracy across both classes)

    * Macro Average:

    * Precision: 0.92
    * Recall: 0.95
    * F1-score: 0.94
    * Weighted Average:

    * Precision: 0.99
    * Recall: 0.99
    * F1-score: 0.99

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

*  This model is great at indentifying healthy loans. It has a precision score of 100%. 

*  Considering that we are dealing with data for credit risk, there is little to no room for error. Each percentage can mean hundreds of thousands to millions of dollars or even greater.

*  I do not recommend this model as a means to identify high risk loans. This model allows for 15% of high risk loans to be missed. This is a large number for a financial instituation to risk. 
