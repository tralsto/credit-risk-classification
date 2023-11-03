# Module 20 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).
--------------------------------------------------------------------------------------------------------
The purpose of this analysis is to create a model to predict a borrowers' creditworthiness for a loan. The model will to run through the data of loans and predict whether or not certain loans would be categorized as a (0) "healthy loan" or a (1) "high-risk loan". Our target values are (0) "healthy loan" and (1) "high-risk loan". The value shown with 'value_counts' are 75036 (0) "healthy" loans and 2500 "high-risk" loans. 

For this Challenge I performed these steps to result in the desired results:
  1. Split the Data into Training and Testing Sets
  2. Create a Logistic Regression Model
  3. Write a Credit Risk Analysis Report

I utilized a Linear Regression model on the original data to test how the model would perform in predicting the loan labels.


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.

  • The model states that the precision of predicting 0 "healthy"     loans is 100% and recall is 99%.
  • This means the model is good about predicting the "healthy" loans almost every single time.
  • The model states the precision of predicting 1 "high-risk" loans is 85% and the recall is 91%.
  • This could pose a problem because this could mean that the model could be predicting false postives in the sense that they are labeling loans "healthy" when they should be labeled "high-risk".

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

  N/A - Did not complete Model 2 as told in class.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
------------------------------------------------------------------------------

As far as I can tell, the prediction of labeling "healthy" loans is much more accurate and reliable than the predicting of the "high-risk" loans. This performance causes a problem as predicting the "high-risk" loans is much more important than predicting the "healthy" loans. For example, it would be an issue if a "high-risk" loan was labeled as a "healthy" loan because the probability of the loan being paid off in the allotted time might be lower than an actual "healthy" loan.