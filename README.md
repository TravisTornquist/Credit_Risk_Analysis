# Credit_Risk_Analysis

## Overview

The purpose of this analysis is to identify the best machine learning model for predicting which loan applicants will be designated as high risk applicants. A good model for predicting risk designation can improve loan processing time by automating some of the decision making required to come to a risk designation.

## Results

Below are the results of each of the tested machine learning models.

- Naive Random Oversampling
  - Accuracy: 65.2%
  - Precision: 1%
  - Recall: 61%
- SMOTE Oversampling
  - Accuracy: 62.3%
  - Precision: 1%
  - Recall: 61%
- Undersampling
  - Accuracy: 51.6
  - Precision: 1%
  - Recall: 60%
- Combination Sampling
  - Accuracy: 64.4%
  - Precision: 1%
  - Recall: 69%
- Balanced Random Forest Classifier
  - Accuracy: 78.7%
  - Precision: 4%
  - Recall: 67%
- Easy Ensemble AdaBoost Classifier
  - Accuracy: 92.5%
  - Precision: 7%
  - Recall: 91%

##Summary

By far, the most accurate machine learning model for this data set is the Easy Ensemble AdaBoost Classifier. While the other models have accuracy scores ranging from 51%-79%, the Easy Ensemble AdaBoost Classifier has an accuracy score of 92.5%. Both the precision and recall are also higher than for any other model.

With a recall score of 91%, there will be relatively few applications incorrectly marked as Low-Risk, therefore this model could allow applicants predicted to be Low-Risk to be automatically approved.

With a precision score of 7%, the Easy Ensemble AdaBoost Classifier will result a large number of applications incorrectly labeled as High-Risk. With that in mind any applicants predicted to be High-Risk would need to be manually reviewed in order to confirm the correct designation.

Provided the cost savings from using the model outweighs any losses from the small number of falsely labeled Low-Risk loans, the Easy Ensemble AdaBoost Classifier should be used.
