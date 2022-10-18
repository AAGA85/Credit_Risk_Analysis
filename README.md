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



## Summary: Evaluation of the performance of the machine learning model

Well, we have built these machine learning models and trained them on some data, so now the question is what is the most accurate model that will help us to reduce the risk for the lending services company. The following is a detail explanation of how to evaluate our model based on what we are expecting.

Classification matrics:

There are four types of outcomes that we can get from the confussion matrix:

a) True positives mean that we have predicted an observation that belongs to a class and it actually belongs to that class.

b) True negatives mean that we have predicted an observation that does not belong to a class and it actually does not belogn to that class.

c) False positives mean that we have predicted an observation that belongs to a class and it actually does not belong to that class

d) False negative mean that we have predicted an obervation that does not belong to a class and it actually belongs to that class

The following diagram illustrates the confusion matrix and how we can interpretate the data that we get from each model: 


<img width="296" alt="confusion matrix" src="https://user-images.githubusercontent.com/106939511/196540002-c2409b3e-882c-4575-9c16-d82c5b760989.png">



The next step once we have classified is to look at the metrics:

a) Accuracy: that means the number of correctly classified data instances over the total numbers of data instances.

b) Precision: means from all the positive predictions, how many are really positive (false positives). 

c) Recall: means from all the real positive data values, how many are predicted positive ( false negatives). 

In our case of study we should evaluate what is worse, false positives or false negatives. Let's evaluate this by revising our case with the 2 undesirable scenarios: 

Scenario 1: Risky loans classified as Non- Risky loans

Scenario 2: Non- Risky loans classsified as Risky loans.

Between these two scenarios, the more undesirable will be Risky loans classified as Non-Risky loans bacause the company doesnt what to lending money to people that cannot pay. Since the impact of errors caused by False positives is assessed to be more significant, it makes sense to select a model taht has a few False positives as possible. In other words, we should use precision instead of recall.


In the following chart we have prepared the comparison between all those models, let's take a look:

<img width="610" alt="table" src="https://user-images.githubusercontent.com/106939511/196544749-a4440a74-8c7a-4bae-b9d3-54b638637b0c.png">


Based on our analysis and the comparison table is clear to see that all models could help us to get the more precision of the risky loans. 





