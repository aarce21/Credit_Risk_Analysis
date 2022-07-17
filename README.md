# Credit Risk Analysis
# Overview
The purpose of the Credit Risk Analysis is to utilize Machine Learning algorithms to evaluate credit risk. The credit data used for this analysis is from Lending Treee and various Machine Learning models were applied to it such as SMOTE, RandomOversampler, SMOTEENN, ClusterCentroids, EasyEnsembleClassifier, and BalancedRandomForestsClassifier. Our goal was to evaluate credit risk based on the data that was already given using Supervised Machine Learning. 

# Results 
Six different Machine Learning Algorithms were applied to the credit risk data. Each of the balanced accuracy scores and the classification reports for each model can be seen below.

## Naive Random Oversampling 
![randomoversampling_balanced](https://github.com/aarce21/Credit_Risk_Analysis/blob/main/images/randomoversampling_balanced.PNG)
![randomoversampling_report](https://github.com/aarce21/Credit_Risk_Analysis/blob/main/images/randomoversampling_report.PNG)

* The Naive Random Oversampling model has a balanced accuracy score of 0.661, meaning it is about 66% accurate at determining the correct credit risk. 
* The high risk precision rate for this model is 0.01, or 1% and has a recall of 0.72. The low precision indicated that there may be a large number of false positives and that scores that were labeled as high risk may have actually been low risk. 
* The low risk precision rate is 1.00, or 100% and the recall is 0.60. 

## SMOTE Oversampling
![smote_balanced](https://github.com/aarce21/Credit_Risk_Analysis/blob/main/images/smote_balanced.PNG)
![smote_report](https://github.com/aarce21/Credit_Risk_Analysis/blob/main/images/smote_report.PNG)

* SMOTE Oversampling returned a balanced accuracy score of 0.658
* The high risk results have a precision rate of 0.01 and a recall of 0.62. 
* The low risk results have a precision of 1.00, meaning the model correctly determined the number of low risk credit, and a recall of 0.69, which is a slight improvement of the recall score using the Naive Random Oversampling model. 

## ClusterCentroids Undersampling 
