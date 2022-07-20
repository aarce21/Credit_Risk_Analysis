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
![cluster_balanced](https://github.com/aarce21/Credit_Risk_Analysis/blob/main/images/cluster_balanced.PNG)
![cluster_report](https://github.com/aarce21/Credit_Risk_Analysis/blob/main/images/cluster_report.PNG)

* The ClusterCentroids model returned a balanced accuracy score of 0.54, lower than the two previous oversampling methods. 
* The high risk results returned a precision of 0.01 and a recall of 0.69.
* The low risk results returned a precision of 1.00 and a recall of 0.40. This low recall rate could indicate there there were a large number of false negatives. 

## SMOTEENN Combination Sampling 
![smoteenn_balanced](https://github.com/aarce21/Credit_Risk_Analysis/blob/main/images/smoteenn_balanced.PNG)
![smoteenn_report](https://github.com/aarce21/Credit_Risk_Analysis/blob/main/images/smoteenn_report.PNG)

* The SMOTEENN model returned a balanced accuracy score of 0.645
* The high risk results also returned a precision rate of 0.01 and a recall of 0.72, which is a slight improvement from the ClusterCentroids model. 
* The low risk results returned a precision of 1.00, just as the other models did, and a recall of 0.57, also an increase from the ClusterCentroids model. 

## Balanced Random Forest Classifier
![brf_balanced](https://github.com/aarce21/Credit_Risk_Analysis/blob/main/images/brf_balanced.PNG)
!![brf_report](https://github.com/aarce21/Credit_Risk_Analysis/blob/main/images/brf_report.PNG)

* The balanced random forest ensemble learned model returned a balanced accuracy score of 0.789, 78.9%
* The high risk results yielded a precision of 0.3 and a recall of 0.70
* The low risk results yielded a precision of 1.00 and a recall of 0.87
* After listing the features in descencing order, the top feature was 'total_rec"prncp'

## Easy Ensemble AdaBoost Classifier
![ee_balanced](https://github.com/aarce21/Credit_Risk_Analysis/blob/main/images/ee_balanced.PNG)
![ee_report](https://github.com/aarce21/Credit_Risk_Analysis/blob/main/images/ee_report.PNG)

* For the easy ensemble classifier, the balanced accuracy score was 0.93, 93%. This is the highest balanced accruacy score we have seen from a model. 
* The high risk results have a precision of 0.09 and a recall of 0.92
* The low risk results also have a precision of 1.00 and a recall of 0.94. 


# Summary
After running a model one of the features that is important to look at is the balanced accuracy score. The closer the balanced accuracy score is to 1, the better it is at classifying a loan application as either high or low risk. After running the Naive Random Oversamplimg, SMOTE, ClusterCentroids, and SMOTEENN models, the Naive Random Oversampling model returned the highest balanced accuracy score of 0.66. The Balanced Random Forest model, with a balanced accuracy score of 78.9%, and the Easy Ensemble model, with a balanced accuracy score of 93%, were then ran. The Easy Ensemble classifier yielded the highest accuracy score of any of the models, meaning it most accurately predicted high and low risk candidates, and this would be my recommendation. This model also had the higest recall for predicting high risk candidates, predicting the true positives at 92%. 

