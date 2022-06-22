# Credit_Risk_Analysis

### Overview and Purpose

The purpose of the analysis is to focus on Supervised Machine Learning and test different models on a large dataset of loans, to determine if the model can predict results for loan approvals and denials.

### Summary

The Supervised Machine Learning performed as followed on the dataset.

#### RandomOverSampler

- Balance Accuracy Score: 60.7%
- Precision: 99%
- Recall: 61%
- F1: 75%

![RandomOverSampler_BAS](https://user-images.githubusercontent.com/98929742/174922132-9d9d39bd-754a-4751-8d2a-8f2824962b44.png)
![RandomOverSampler_Classification_Report](https://user-images.githubusercontent.com/98929742/174922127-324fc217-de2a-4463-a82e-0171a4a64834.png)


#### SMOTE

- Balance Accuracy Score: 63.3%
- Precision: 99%
- Recall: 67%
- F1: 80%

![SMOTE_BAS](https://user-images.githubusercontent.com/98929742/174922159-652d47dd-975d-4f3f-b791-75f8880a92ce.png)
![SMOTE_Classification_Report](https://user-images.githubusercontent.com/98929742/174922165-6ee5ecae-e8a2-4b44-875e-a836fce1456b.png)


#### ClusterCentroids

- Balance Accuracy Score:51.4%
- Precision: 99%
- Recall: 48%
- F1: 64%

![ClusterCentroids_BAS](https://user-images.githubusercontent.com/98929742/174922194-1839a45a-c454-406d-8771-e230fae62f91.png)
![ClusterCentroids_Classification_Report](https://user-images.githubusercontent.com/98929742/174922197-ada1cd91-9f51-4cff-9f50-1c145b7da657.png)


##### SMOTEENN

- Balance Accuracy Score: 65.8%
- Precision: 99%
- Recall: 56%
- F1: 71%

![SMOTEENN_BAS](https://user-images.githubusercontent.com/98929742/174922283-786941c7-7221-4952-aae5-01e6a698cf3b.png)
![SMOTEENN_Classification_Report](https://user-images.githubusercontent.com/98929742/174922284-4086b38b-b14c-4e68-9d31-f8c63a7d2f21.png)


#### BalancedRandomForestClassifier

- Balance Accuracy Score: 79.2%
- Precision: 99%
- Recall: 90%
- F1: 95%

![RandomOverSampler_BAS](https://user-images.githubusercontent.com/98929742/174922313-0091d689-8e2d-486c-8d57-bbc85515c600.png)
![RandomOverSampler_Classification_Report](https://user-images.githubusercontent.com/98929742/174922322-1dfe7d13-8a35-49cc-9fc8-2d00cf6dc4c4.png)


#### EasyEnsembleClassifier

- Balance Accuracy Score: 91.4%
- Precision: 99%
- Recall: 94%
- F1: 97%

![EasyEnsembleClassifier_BAS](https://user-images.githubusercontent.com/98929742/174922352-adb5ba5a-d336-4533-bff5-ae535b53f33a.png)
![EasyEnsembleClassifier_Classification_Report](https://user-images.githubusercontent.com/98929742/174922360-fd652c88-2a80-4602-916d-84d95b43f73d.png)


### Recommendation

**Sensitivity / Recall**

- 92% of them were detected and properly classified as high-risk.

**Precision**

- 9% high-risk.
- 91% high-risk predictions results on false positives

The model yields a High a Recall **(%92)** and is more important. A test with high sensitivity means few false negatives, though there may be a high number of false positives. In this context, false positives are preferable to false negatives. It is better to rule out false positive diagnoses than to miss patients who actually have cancer.
