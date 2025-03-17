# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
    The purpose of this analysis is to determine if the Logistic Regression Learning model can better predict healthy 
    verses high risk loans using the original or resampled dataset. 

* Explain what financial information the data was on, and what you needed to predict.
    The dataset consisted of information for 77,536 loans that inlcuded columns rated to loan size, interest rate, borrower income, debt to income ratio,
    number of accounts, derotatory marks, total debt and loan status. 
    
* Describe the stages of the machine learning process you went through as part of this analysis.
    The stages of the machine learning process included the following:
        1. Prepared the data- imported the file, established the DataFrame, evaluated the columns and features.
        
        2. Separated the data into features and labels - the labeled items I'm attempting to predict, are the status of the loan
           healthy(0) or high-risk (1). The remaining items are used to train and test the model.
        
        3. Used the train_test_split function to separate the features and labels data into the training and testing datasets. 
        
        4. Imported the machine learning model from the library - imported LogisticRegression from SKLearn.
            a. Iniated the model
            b. Fit the model using the training data.
            c. Used the moded to make predictions using the feature test data.
            d. Evaluated the predictions- the evalutions were done by calculating and comparing metrics like the accuracy,
               confusion matrix, and a classification report.


* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).
    The Machine Learning Method was used and the primary model used was the LogisticRegression model along with Train_test_split from SKLearn.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model- Logistic Regression:
    1. Accuracy Score: 99%  
    
    2. Precision Scores: 
        Class 0(Healthy Loans) - 100%
        Class 1(High-Risk Loans) -84%
    
    3. Recalls
        Class 0(Healthy Loans) - 99%
        Class 1(High-Risk Loans) -94%

## Summary

*  The model does an eceptionally good job in predicting Healthy Loan (0) loan types with precison scores of 100% and with a recall score of 99%.
   The model is also good at predicting the values of high risk loans, with a precision of 84% and recall of 94%. 
   Overall, the Logistic Regression model does a good job of predicting both healthy and high-risk loans. 
