# Module 12 Report Template

## Overview of the Analysis

In this analysis, the focus is on utilizing machine learning methods, particularly Logistic Regression, to evaluate credit risk in lending activities. The dataset under scrutiny contains historical data from a peer-to-peer lending service, encompassing borrower details, loan attributes, and repayment statuses. 

The primary objective is to develop a model capable of discerning the creditworthiness of borrowers, crucial for lending companies to mitigate losses associated with defaulted loans. The key variable of interest is the `loan_status`, categorized as either 0 for healthy loans (low-risk) or 1 for non-healthy loans (high-risk). 

Initial exploration reveals a significant imbalance in the dataset, with a notable surplus of healthy loans compared to non-healthy ones. The analysis progresses through several stages of the machine learning process. It commences with data exploration and preprocessing, followed by model selection, where Logistic Regression emerges as the algorithm of choice due to its suitability for binary classification tasks and interpretability. 

The evaluation of the initial model reveals performance metrics such as accuracy score, recall, and confusion matrix, highlighting the challenges posed by imbalanced data. To address this issue, the dataset undergoes resampling using the RandomOverSampler module to rebalance the classes. Subsequently, the Logistic Regression model is retrained with the resampled data and reassessed for performance improvement. 

Through these steps, the analysis aims to provide insights into credit risk prediction and demonstrate the efficacy of data resampling techniques in enhancing model performance for imbalanced datasets.

## Results

* Machine Learning Model 1:
    * The model generated an accuracy score of 95% but could be improved due to the dataset being imbalanced.
    * The Logistic Regression model fitted with the Imbalanced DataSet predicted healthy loans 100% of the time and predicted non-healthy loans 85% of the time
    * According to the models recall scores, the model made 1% of mistakes when predicting healthy loans and made 9% of mistakes when predicted non-healthy loans


## Summary

A lending company might want a model that requires classifying healthy loans and non-healthy loans correctly most of the time: healthy loans being identified as a non-healthy loan might be more costly for a lending company since it might cause the loss of customers; whereas, non-healthy loans being identified as a healthy loan might also be more costly for a lending company due to the loss of funds being provided by the lender

AKA: The lending company would most likely want fewer False Positives due to the high possibility of a lender loosing provided funds when classifying non-healthy loans as healthy. The data below is shown in the confusion matrices which indicates how many healthy/non-healthy loans the model predicted correctly or incorrectly.

Model false positives:

56 (FALSE POSITIVES) --> The actual value is healthy and the predicted value is non-healthy

102 (FALSE NEGATIVES) --> The actual value is non-healthy and the predicted value is healthy

Based off of this analysis criteria, I wouldn't recommend this Logisitics Regression model without oversampling the data set first to control for mistakes when classifying non-healthy loans.
