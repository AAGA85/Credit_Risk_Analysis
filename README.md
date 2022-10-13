# Credit_Risk_Analysis

# Overview

A peer to peer lending services company  wants to use machine learning to predict credit risk. Upper management believes that this will provide a quicker and more realiable loan experience. The company wants us to assist the lead Data Scientist in implementing this plan. To do that we will evaluate several machine learning models to predict credit risk.

In this challenge we will use the credit card credit dataset from LendingClub and perform the analysis in the following way:

a) **Oversampling** data by using the *RandomOverSampler* and *SMOTE* algorithms

b) **Undersampling** data by using the *ClusterCentroids* algorithm 

c) **Combinatorial approach of over-and undersampling** using the *SMOTEENN* algorithm

d) **New machine learning models**: *BalanceRandomForestClassifier* and *EasyEnsambleClassifier*


# Results

## Oversampling

![naive random](https://user-images.githubusercontent.com/106939511/195468017-83834dbe-9eaf-447c-a7d7-2d63f7f53cd9.png)




![smote](https://user-images.githubusercontent.com/106939511/195468041-a104a548-3a3c-4bf6-9e2b-c8a12ed0f9c0.png)



## Undersampling: ClusterCentroids

![undersampling](https://user-images.githubusercontent.com/106939511/195476014-4b03e63b-ed23-426b-806c-018ddbc85573.png)


## Combination (Over and Under) Sampling: SMOTEENN


![combination](https://user-images.githubusercontent.com/106939511/195476084-4d9bdada-eaf4-4c96-9434-9e5d03256478.png)


## Ensemble Learners

![balance](https://user-images.githubusercontent.com/106939511/195476113-4a716328-a34d-432f-951a-6e1c06c16750.png)


![easy](https://user-images.githubusercontent.com/106939511/195476164-8a3ac5e7-fc0b-4967-8e01-f273bca28e81.png)



## Summary

In the following chart we have prepared the comparison between all those models, let's take a look:

![table](https://user-images.githubusercontent.com/106939511/195478612-61af954c-f1f6-4cb1-b450-d7561459c924.png)

