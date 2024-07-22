# credit-risk-classification
Supervised learning project of a model based on loan risk. Historical lending activity used to build a model that identifies the creditworthiness of borrowers.

# Module 12 Report 

## Overview of the Analysis

* The purpose of this analysis is to create and evaluate the accuracy of a data model that predicts the credity worthiness of potential borrowers   from peer-to-peer lending services based on the historical lending activity. 
* A machine learning model was used to determine which loans are healthy (low-risk) or non-healthy (high-risk) based on the loan status.
* The Logistic Regression Algorithm used in a classification model helps to predict the probability of the target variable.

* The financial information provided in the dataset consists of: 

    - Loan size: The amount of money borrowed by the applicant.
    - Interest rate: The annual interest rate charged on the loan.
    - Borrower income: The annual income of the loan applicant.
    - Debt-to-income ratio: The ratio of the borrower's total debt to their annual income.
    - Number of accounts: The total number of credit accounts held by the borrower.
    - Derogatory marks: The number of negative items (e.g., late payments, bankruptcies) on the borrower's credit report.
    - Total debt: The borrower's total outstanding debt, excluding the loan being applied for.Explain what financial information the data was on, and   what you needed to predict.

* The target variable to be predicted is loan_status, which indicates if loans are healthy (low-risk) or non-healthy (high-risk). In this case, "0" is assumed to be healthy and "1" as non-healthy.


* Describe the stages of the machine learning process you went through as part of this analysis.

    Data Preparation: Early stage that involves cleaning and pre-processing the data. This might include handling missing values, encoding categorical variables (if any), and potentially scaling the numerical features for a better model performance.

    Splitting Data into Training and Testing Sets: This stage involves preparing the data for model training and evaluation. By splitting the data, we ensure the model is trained on a portion of the data (training set) and evaluated on unseen data (testing set). This prevents overfitting and provides more realistic assessment of the model's performance.

    Model Training: Using training data (X_train and y_train) to fit the logistic regression model. This trains the model to learn the relationship between the financial information and loan status.

    Model Evaluation: The testing data (X_test and y_test) is used to evaluate the model's performance. This involves calculating metrics like accuracy, precision, recall, and F1-score to assess how well the model generalizes to unseen data.

* Methods & Algorithms

Logistic regression is a statistical method that can analyze binary data (like loan status) and predict the probability of an outcome based on one or more predictor variables (the financial information). After fitting a logistic regression model to the data, it can estimate the relationship between the financial information of loan applicants and their loan status. 

## Results

* Accuracy scores, precision and recall scores of machine learning model

* Machine Learning Model Classification Report Summary:
   
    * Accuracy: 92%
    * Precision:
    * Healthy Loans (low-risk): 1.00
    * Non-Healthy Loans (high-risk): 0.85
    * Recall:
    * Healthy Loans (low-risk): 0.99
    * Non-Healthy Loans (high-risk): 0.91

    Accuracy shows that 92% of loans were correctly classified (healthy or non-healthy).
    Regarding precision: The model is excellent at identifying healthy loans (100% precision), with almost no false positives.
    Non-healthy loan identification is good (85% precision), although there's a chance of false positives.
    Recall: The model captures most healthy loans (99% recall), missing just a few. Most non-healthy loans are identified (91% recall), with a chance of missing some risky ones, or false negatives.

## Summary

In order to acquire a more precise and comprehensive understanding of the model's performance, it's important to consider all the metrics together. The overall accuracy is high, although the precision for non-healthy loans is lower than the precision for healthy ones. This could be a crucial factor depending on the specific application in the company. A higher precision for non-healthy loans might be desirable, to be able to avoid approving risky loans. 


