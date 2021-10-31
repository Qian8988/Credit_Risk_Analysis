# Credit_Risk_Analysis


Module 17 Challenge



## Overview of the loan prediction risk analysis:

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we’ll need to employ different techniques to train and evaluate models with unbalanced classes. Use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, I’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, I’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, I’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once done, I’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.



## Results:

Deliverable 1: Use Resampling Models to Predict Credit Risk

Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk

Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk

Deliverable 4: A Written Report on the Credit Risk Analysis (README.md)

[credit_risk_resampling.ipynb](credit_risk_resampling.ipynb)

[credit_risk_ensemble.ipynb](credit_risk_ensemble.ipynb)


### 1.	RandomOverSample: 

the accuracy score is 62%, the precision for the high_risk loans is at 1% with 64% sensitivity and the precision overall is 99% with a sensitivity of 62%.

<img width="384" alt="1" src="https://user-images.githubusercontent.com/86527347/139600659-92c40bdf-9efe-41c5-b16d-4fad66e07eba.png">



### 2.	SMOTE: 

the accuracy score is 63%, the precision for the high_risk loans is at 1% with 64% sensitivity and the precision overall is 99% with a sensitivity of 62%.

<img width="346" alt="2" src="https://user-images.githubusercontent.com/86527347/139600660-3a7151f1-88f6-4626-82a0-bb580fa52d9e.png">



### 3.	ClusterCentroids: 

the accuracy score is 53%, the precision for the high_risk loans is at 1% with 61% sensitivity and the precision overall is 99% with a sensitivity of 45%.

<img width="346" alt="3" src="https://user-images.githubusercontent.com/86527347/139600661-e6a51e93-2593-498c-9d87-3cd182374e48.png">


### 4.	SMOTEENN: 

the accuracy score is 64%, the precision for the high_risk loans is at 1% with 69% sensitivity and the precision overall is 99% with a sensitivity of 60%..

<img width="396" alt="4" src="https://user-images.githubusercontent.com/86527347/139600663-c9279733-1c9b-4f98-9d68-4689ef585e8c.png">




### 5.	BalancedRandomForestClassifier: 

the accuracy score is 79%, the precision for the high_risk loans is at 3% with 70% sensitivity and the precision overall is 99% with a sensitivity of 87%.

<img width="382" alt="5" src="https://user-images.githubusercontent.com/86527347/139600664-b7164852-4d64-407b-a1ce-03d5e116b167.png">

### 6.	EasyEnsembleClassifier: 

the accuracy score is 93%, the precision for the high_risk loans is at 9% with 92% sensitivity and the precision overall is 99% with a sensitivity of 94%.


<img width="361" alt="6" src="https://user-images.githubusercontent.com/86527347/139600658-e4da674f-4fdd-4dbf-8361-3008b8cc2343.png">


## Summary:

The Easy Ensemble Classifier model provides a recall of 92%, is the highest of all models. Which means that using Easy Ensemble Classifier will help detect almost all high risk credit. While other models provide a low precision, with those models a bank has more chance to falsely detect a high risk loan and might missing some business opportunities. That is why I would recommend the bank to use the Easy Ensemble Classifier model to predict credit risk.
