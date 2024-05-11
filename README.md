Credit-Risk-Classification

Machine learning techniques are used to analyze a dataset of historical lending activity from a peer-to-peer lending services company to build a model that can identify the creditworthiness of borrowers.

Overview of the Analysis

Factors considered in the analysis included data on:
the size of the loan
its interest rate
the borrower's income
the debt to income ratio
the number of accounts the borrower held
derogatory marks against the borrower
the total debt

The dataset (77,536 data points) was split into training and testing sets. The training set was used to build an initial logistic regression model using the LogisticRegression module from scikit-learn. The purpose of the model was to determine whether a loan to the borrower in the testing set would be low- or high-risk and results are summarized below.

This intial model was drawing from a dataset that had 75,036 low-risk loan data points and 2,500 high-risk data points. 
Results
Logistic Regression:

Precision: 93% (an average--in predicting low-risk loans, the model was 100% precise, though the model was only 87% precise in predicting high-risk loans)
Accuracy: 94%
Recall: 95% (an average--the model had 100% recall in predicting low-risk loans, but 89% recall in predicting high-risk loans)

If the goal of the model is to determine the likelihood of high-risk loans, then the model scores less than 90% and should not be used. However if used for only low risk-loans than the model was extremely precise 
