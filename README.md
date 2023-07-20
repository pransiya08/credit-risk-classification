# Credit Risk Classification

## Overview of the Analysis
This credit risk analysis is done for the lending company to use in identifying high or low risk loans. Using the historical lending activities, a model, based on Logistic Regression, is built to identify the creditworthiness of borrowers.

This analysis utlises the lending data of the borrowers, including their loan size, the interest rate they have on their loan, their income, debt-to-income ratio, the number of accounts they have, if they have any derogatory remarks, and the total debt that they have. Using all these factors, the model aims to predict the loan status, if it is healthy or a high-risk loan, of the current and future borrowers. 

Essentially, if the model predicts that the loan is healthy, the lending company is more inclined to approve their loan as they will be considered as a low-risk borrower. However, if the model predicts that it is a high-risk loan, then this will flag the company that the loan is a high-risk one and they will be more inclined to decline the loan.

The target (loan status) was first identified from the lending data and the rest were considered as features, which are all considered and analysed to predict the loan status. Then, all of the lending data were split into the training data and testing data. The training data were fit into the Logistic Regression model, then the test data was used in the trained model to predict the loan status. These predictions were then analysed using the confusion matrix, and ultimately, by analysing its precision and recall scores using the classification report.

## Results
* Machine Learning Model: Logistic Regression
    * Precision: [0] - '1.00'   | [1] - '0.85'
    
        The model predicts healthy loans ('0') correctly all the time, whereas, predicting high-risk loans (1) is only correct 85% of the time.

    * Recall: [0] - '0.99'   | [1] - '0.91'
    
        Out of 100 predictions of healthy loans, 99 of them are actually health. However, in predicting the high-risk loans, out of the 100 predictions, they tag 9 of them as high-risk when it should be a healthy loan

    * Accuracy: '0.99'
    
        In terms of accuracy, out of all the predictions that the model made, 99% of them are correctly predicted.       

## Summary

In conclusion, the Logistic Regression model is good to use to predict the healthy loans/low-risk borrowers. However, depending on the risk-appetite of the lending company, they should be careful in using this model in predicting the high-risk loans as they might missed out on some borrowers that are actually low-risk and tag them as high-risk borrowers.