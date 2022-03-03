# Credit_Risk_Analysis
## Project Overview
In this project we applied our knowledge of machine learning to assist our client in creating a viable model that can accurately predict credit card risk. Utilizing a credit dataset from LendingClub, a peer-to-peer lending services company, we applied different techniques to train and evaluate our models to see which we would be able to recommend.
- Oversample the data using the **RandomOverSampler** and **SMOTE** algorithms.
- Undersample the data using the **ClusterCentroids** algorithm.
- Use a combinatorial approach of over- and undersampling using the **SMOTEENN** algorithm.
- Compare two machine learning models that reduce bias, **BalancedRandomForestClassifier** and **EasyEnsembleClassifier**.

## Resources
- Data Source: LoanStats_2019Q1.csv
- Software: Python & Jupyter Notebook 

## Results
### RandomOverSampler Model
<p align="center">
<img width="338" alt="OverSample_balance" src="https://user-images.githubusercontent.com/93271297/156622977-e1972ec2-27e3-4732-99cf-580bf2d17cc6.png"><img width="352" alt="OverSample_Matrix" src="https://user-images.githubusercontent.com/93271297/156622999-ee618e70-3b44-45c2-8cd9-4ba37f2bb453.png"><img width="712" alt="OverSample_report" src="https://user-images.githubusercontent.com/93271297/156623004-9a8588de-58d3-4375-9a36-4d8d9733dd4a.png">
</p>

- The balanced accuracy score is **~65%**
- The high-risk precision was **.01 (1%)** where as the low-risk precision was **1 (100%)** which indicates that the low-risk classification from the model is far more reliable than the high-risk classification (i.e. The model classifies an applicant as high-risk or low-risk, how likely is it that the classification is correct) 
- The high-risk recall was **.61 (61%)** where as the low-risk recall was **.68 (68%)** which indicates that the model was relatively accurate in correctly classifying an applicant as low-risk or high-risk (i.e. of those classified as low-risk or high-risk, how many of those classifications were correctly made)

### SMOTE Model
<p align="center">
<img width="342" alt="SMOTE_balance" src="https://user-images.githubusercontent.com/93271297/156624132-eebbd4ac-f4cd-4b36-be29-1f8c479b0c24.png"><img width="348" alt="SMOTE_matrix" src="https://user-images.githubusercontent.com/93271297/156624144-764ec59d-27c3-42a1-89e0-9f9383647f59.png"><img width="703" alt="SMOTE_report" src="https://user-images.githubusercontent.com/93271297/156624159-24480721-eec0-485c-ad7c-be77867f6b2b.png">
</p>

- The balanced accuracy score is **~62%**
- The high-risk precision was **.01 (1%)** where as the low-risk precision was **1 (100%)** which indicates that the low-risk classification from the model is far more reliable than the high-risk classification (i.e. The model classifies an applicant as high-risk or low-risk, how likely is it that the classification is correct) 
- The high-risk recall was **.61 (61%)** where as the low-risk recall was **.64 (64%)** which indicates that the model was relatively accurate in correctly classifying an applicant as low-risk or high-risk (i.e. of those classified as low-risk or high-risk, how many of those classifications were correctly made)

### ClusterCentroids Model
<p align="center">
<img width="336" alt="cluster_balance" src="https://user-images.githubusercontent.com/93271297/156624982-5bf7b28a-40c7-467e-8fee-5a2ab701ffd9.png"><img width="346" alt="cluster_matrix" src="https://user-images.githubusercontent.com/93271297/156624997-8e6b6f8a-0a8c-48cf-99c6-a9fe4fd92b99.png"><img width="704" alt="cluster_report" src="https://user-images.githubusercontent.com/93271297/156625002-593bc7d1-3588-4825-b435-1b713524ac89.png">
</p>

- The balanced accuracy score is **~51%**
- The high-risk precision was **.01 (1%)** where as the low-risk precision was **1 (100%)** which indicates that the low-risk classification from the model is far more reliable than the high-risk classification (i.e. The model classifies an applicant as high-risk or low-risk, how likely is it that the classification is correct) 
- The high-risk recall was **.60 (60%)** where as the low-risk recall was **.43 (43%)** which indicates that the model was more accurate in correctly classifying an applicant as high-risk than it was as low-risk (i.e. of those classified as low-risk or high-risk, how many of those classifications were correctly made)

### SMOTEENN Model
<p align="center">
<img width="335" alt="SMOTEEN_balance" src="https://user-images.githubusercontent.com/93271297/156626402-f69e2d56-045b-4aaf-914e-f9df02fc5b33.png"><img width="347" alt="SMOTEEN_matrix" src="https://user-images.githubusercontent.com/93271297/156626423-4ac30f06-601e-4f66-886f-473a0be91810.png"><img width="701" alt="SMOTEEN_report" src="https://user-images.githubusercontent.com/93271297/156626432-c2c6f8d4-6141-4b80-999f-da027d78deb8.png">
</p>

- The balanced accuracy score is **~63%**
- The high-risk precision was **.01 (1%)** where as the low-risk precision was **1 (100%)** which indicates that the low-risk classification from the model is far more reliable than the high-risk classification (i.e. The model classifies an applicant as high-risk or low-risk, how likely is it that the classification is correct) 
- The high-risk recall was **.71 (71%)** where as the low-risk recall was **.58 (58%)** which indicates that the model was more far more accurate in correctly classifying an applicant as high-risk than it was as low-risk (i.e. of those classified as low-risk or high-risk, how many of those classifications were correctly made)

### Balanced Random Forest Classifier
<p align="center">
<img width="335" alt="Forest_balance" src="https://user-images.githubusercontent.com/93271297/156634624-ea113187-a491-4479-911e-ab42a9d51d5e.png"><img width="343" alt="Forest_matrix" src="https://user-images.githubusercontent.com/93271297/156634643-d3b79d61-585f-4434-b0f0-a9e03ef6aee3.png"><img width="707" alt="Forest_report" src="https://user-images.githubusercontent.com/93271297/156634655-fe5b1e62-2370-4f81-bd84-3772041b6304.png">
</p>

- The balanced accuracy score is **~78%** which is a subsantial improvement from previous models
- The high-risk precision was **.04 (4%)** where as the low-risk precision was **1 (100%)** which indicates that the low-risk classification from the model is far more reliable than the high-risk classification (i.e. The model classifies an applicant as high-risk or low-risk, how likely is it that the classification is correct) 
- The high-risk recall was **.67 (67%)** where as the low-risk recall was **.91 (91%)** which indicates that the model was almost perfectly accurate in correctly classifying an applicant as low-risk than it was as high-risk (i.e. of those classified as low-risk or high-risk, how many of those classifications were correctly made)

### Easy Ensemble AdaBoost Classifier
<p align="center">
<img width="337" alt="ensemble_balance" src="https://user-images.githubusercontent.com/93271297/156646751-036db072-c96b-4707-9c86-eefe7d266b0c.png"><img width="342" alt="ensemble_matrix" src="https://user-images.githubusercontent.com/93271297/156646764-4ac13055-c7a3-4c9d-8603-287990592894.png"><img width="704" alt="ensemble_report" src="https://user-images.githubusercontent.com/93271297/156646773-9434f15e-6398-4406-bbac-ad04702bf71e.png">
</p>

- The balanced accuracy score is **~93%** which is the best score across all models
- The high-risk precision was **.07 (7%)** where as the low-risk precision was **1 (100%)** which indicates that the low-risk classification from the model is far more reliable than the high-risk classification (i.e. The model classifies an applicant as high-risk or low-risk, how likely is it that the classification is correct) 
- The high-risk recall was **.91 (91%)** where as the low-risk recall was **.94 (94%)** which indicates that the model was almost perfectly accurate in classifying all applicants correctly as low-risk and as high-risk (i.e. of those classified as low-risk or high-risk, how many of those classifications were correctly made)

## Summary
After completing our training and evaluation of our models used to perform the credit risk analysis, it is evident that they all show weak precision in determining if a credit risk is high. The Ensemble Classifiers showed a solid level of improvement especially in terms of the sensitivity for the high-risk applicants. The Easy Ensemble AdaBoost Classifier model had a recall of 92% meaning it detects almost all high-risk applicants. However, with a low precision, a lot of low-risk applicants are still falsely classified as high-risk which would penalize the lender's strategy and infer on its revenue by missing those business opportunities. If a recommendation had to be made, I would recommend the Easy Ensemble AdaBoost Classifier model but ultimately I do not believe any of the models performed in such a way that would leave the client feeling confident in its results.
