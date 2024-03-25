# Module 12 Report Template

## Overview of the Analysis

In this analysis, the focus is on utilizing machine learning methods, particularly Logistic Regression, to evaluate credit risk in lending activities. The dataset under scrutiny contains historical data from a peer-to-peer lending service, encompassing borrower details, loan attributes, and repayment statuses. 

The primary objective is to develop a model capable of discerning the creditworthiness of borrowers, crucial for lending companies to mitigate losses associated with defaulted loans. The key variable of interest is the `loan_status`, categorized as either 0 for healthy loans (low-risk) or 1 for non-healthy loans (high-risk). 

Initial exploration reveals a significant imbalance in the dataset, with a notable surplus of healthy loans compared to non-healthy ones. The analysis progresses through several stages of the machine learning process. It commences with data exploration and preprocessing, followed by model selection, where Logistic Regression emerges as the algorithm of choice due to its suitability for binary classification tasks and interpretability. 

The evaluation of the initial model reveals performance metrics such as accuracy score, recall, and confusion matrix, highlighting the challenges posed by imbalanced data. To address this issue, the dataset undergoes resampling using the RandomOverSampler module to rebalance the classes. Subsequently, the Logistic Regression model is retrained with the resampled data and reassessed for performance improvement. 

Through these steps, the analysis aims to provide insights into credit risk prediction and demonstrate the efficacy of data resampling techniques in enhancing model performance for imbalanced datasets.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
