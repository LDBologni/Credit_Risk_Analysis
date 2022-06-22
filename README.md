# Credit_Risk_Analysis - Module 17 - Challenge

### Overview and Purpose

The purpose of the analysis is to focus on a large dataset of loans. Using this dataset we will deploy our knowledge of Supervised Machine Learning and test different models to see if we can achieve acceptable results for loan approvals and denials.

### Summary

Overall the use of Supervised Machine Learning did not perform very well on our dataset. Assessing Credit risks cannot have F1 scores between 64% and 80%. Even using more sophisticated modeling like BalancedRandomForestClassifier and EasyEnsembleClassifier didn't fair much better with 95% and 97% F1 scores. 

High risk lines of credit offer companies better profit margins. When the F1 score for High risk lines of credit tops out at 14%, different ways of assesing credit risks need to be tried.

* RandomOverSampler

Balance Accuracy Score: 60.7%
Precision: 99%
Recall: 61%
F1: 75%

* SMOTE

Balance Accuracy Score: 63.3%
Precision: 99%
Recall: 67%
F1: 80%

* ClusterCentroids

Balance Accuracy Score:51.4%
Precision: 99%
Recall: 48%
F1: 64%

* SMOTEENN

Balance Accuracy Score: 65.8%
Precision: 99%
Recall: 56%
F1: 71%

* BalancedRandomForestClassifier

Balance Accuracy Score: 79.2%
Precision: 99%
Recall: 90%
F1: 95%

* EasyEnsembleClassifier

Balance Accuracy Score: 91.4%
Precision: 99%
Recall: 94%
F1: 97%

