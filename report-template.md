# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Purpose of the analysis:  Test two logistic regression models to determine accuracy, actual values (true negatives, false negatives, false positives and true positives), percision and recall. 
* Financial information included in the data was loan size, interest rate, borrower income, debt to income ratio, number of accounts, derogatory marks, total debt and loan status.  Loan status was dropped from the training model to decrease bias that would be introduced with inclusion.
* Overall the data set included 75,036 occurances of healthy loans and 2,500 of high-risk loans.  The oversampling model harmonized both types of loans to 56,271 occurances. 
* Through a multistep process data was split into training and testing datasets, models were fit and then a prediction model was run.  After model was run the preformance was evaluated for accuracy, actual values, percision and recall. An additional step was needed for the oversampling model. 
* The logistic regression evaluated the relationship between health and high-risk loans and made predictions after a simple model was preformance was evaluated a oversampleing method was used to correct for the bias created by having more healthy loans in the dataset than high-risk loans. Oversampling preseved the data present in the healthy loan category and randomly duplicated data from the high-risk loan category.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Simple Model 1:
  *  Accuracy: 95%
  *  Precision: 99% (Healthy Loan), 91% (High-risk Loan)
  *  Recall: 100% (Healthy Loan), 85% (High-risk Loan) 



* Machine Learning Model 2:
  * Oversampling Model 2:
  *  Accuracy: 99%
  *  Precision: 99% (Healthy Loan), 99% (High-risk Loan)
  *  Recall: 100% (Healthy Loan), 84% (High-risk Loan) 

## Summary
* Overall the simple model had 95 percent accuracy however recall for high-risk loans is 91 percent (99% for healthy loans). This leaves more risk in the model for false negatives than is optimal and will over predict healthy loans in cases of high-risk loans. 
* Overall the oversampling model predicts with more than 99 percent accuracy. The oversampled data increases the recall to 99 percent while maintaining a similar percision score. This therefore reduces the likelyhood of predicting false negatives, that is classifing high-risk loans as healthy lones.
* From the prespective of the lender it is more important to predict false negatives, in other words when the model gives the wrong prediction of the loans that are risky. This error will lead to bad loans being identified as healthy. 

The recommended model for this dataset is the oversampling method.  This increase the likelyhood of identifying risky loans. 
