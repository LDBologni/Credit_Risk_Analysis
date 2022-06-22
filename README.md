# Credit_Risk_Analysis - Module 17 - Challenge

### Overview and Purpose

This analysis focuses on a large dataset of loans. Using this dataset we will deploy our knowledge of Supervised Machine Learning and test different models to see if we can achieve acceptable results for loan approvals and denials.

### Results

Below are the results for the six different machine learning models. The different models use one of each of the following approaches; oversampling, undersampling, or combinatorial.

### Resampling Models
* RandomOverSampler

![RandomOverSampler_Con_Matrix](https://user-images.githubusercontent.com/88510296/145288821-55fd9bc6-a949-4612-aff0-f794e2d9d297.png)

![RandomOverSampler_BAS](https://user-images.githubusercontent.com/88510296/145282862-1dd3ecaf-6e82-4648-b8e1-963d010421a0.png)
![RandomOverSampler_Classification_Report](https://user-images.githubusercontent.com/88510296/145282900-8f27c178-e650-4cda-a833-eb1716f00eed.png)
 
* SMOTE

![SMOTE_Con_Matrix](https://user-images.githubusercontent.com/88510296/145288855-f33bd250-1bfd-4a25-a555-2594f07c31f6.png)

![SMOTE_BAS](https://user-images.githubusercontent.com/88510296/145282930-4e234125-f600-4c7d-9256-4cfb64e14aed.png)
![SMOTE_Classification_Report](https://user-images.githubusercontent.com/88510296/145282943-56b4514a-bb0a-4693-b447-4454beec7a8c.png)
 
* ClusterCentroids

![ClusterCentroids_Con_Matrix](https://user-images.githubusercontent.com/88510296/145288902-9a6f2a80-8aa7-4760-a600-7bf4af93446c.png)

![ClusterCentroids_BAS](https://user-images.githubusercontent.com/88510296/145282957-a566a3dd-52fa-4ad0-a05d-bc5cb6ea4c19.png)
![ClusterCentroids_Classification_Report](https://user-images.githubusercontent.com/88510296/145282973-baaa6d48-0a86-41d5-8053-89d63ccee3b7.png)

### SMOTEENN algorithm
* SMOTEENN = SMOTE (Synthetic Minority Over-sampling Technique) + EEN (Edited Nearest Neighbor)

![SMOTEENN_Con_Matrix](https://user-images.githubusercontent.com/88510296/145288930-2ede4e63-6bfb-42da-817a-768aabc0b182.png)

![SMOTEENN_BAS](https://user-images.githubusercontent.com/88510296/145283020-64022791-9879-45d6-8c3d-90e832e80ac8.png)
![SMOTEENN_Classification_Report](https://user-images.githubusercontent.com/88510296/145283034-fea2028c-174d-4b69-af04-754510f9d8e2.png)

### Emsemble Classifiers
* BalancedRandomForestClassifier

![BalancedRandomForest_Con_Matrix](https://user-images.githubusercontent.com/88510296/145288970-7ece86f5-c1e9-4271-b5d3-0e16e1621139.png)

![BalancedRandomForest_BAS](https://user-images.githubusercontent.com/88510296/145283049-89331ac2-5ac1-4a62-8f26-440e2fbe63ed.png)
![BalancedRandomForest_Classification_Report](https://user-images.githubusercontent.com/88510296/145283064-9490d838-6cb6-4b4a-aa64-400f95b0638f.png)

* EasyEnsembleClassifier

![EasyEnsembleClassifier_Con_Matrix](https://user-images.githubusercontent.com/88510296/145289004-38d338d9-1189-42b3-9efb-dbc105e5c916.png)

![EasyEnsembleClassifier_BAS](https://user-images.githubusercontent.com/88510296/145283090-8e711d61-e6d0-4263-b984-0e5a6d309699.png)
![EasyEnsembleClassifier_Classification_Report](https://user-images.githubusercontent.com/88510296/145283104-5c59a0f8-1aea-4dd5-ace1-010558ad4e44.png)

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

Web Link: (https://github.com/ezra-deutsch/M17_Credit_Risk_Analysis)
