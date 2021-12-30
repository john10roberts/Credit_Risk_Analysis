# Credit_Risk_Analysis
 Credit_Risk_Analysis

## Overview of Project
Using the dataset, we have received from LendingClub, a peer-to-peer lending services company, we have oversampled the data using the RandomOverSampler and SMOTE algorithims, and undersampled using the ClusterCentroids algorithm. Then we have used a combined approach of over/undersampling using the SMOTEENN algorithm. Lastly, we have compared two additional machine learning models to reduce bias the BalancedRandomForestClassifier and EasyEnsembleClassifier. The following is an evaluation of those models. 

## Results
### RandomOverSampler
* Balanced Accuracy - 64%
* High Risk Precision - 1%
* High Risk Sensitivity - 72%
* High Risk F1 - 2%
* Low Risk Precision - 100%
* Low Risk Sensitivity - 56%
* Low Risk f1 - 72%

![RandomOverSampler](https://github.com/john10roberts/Credit_Risk_Analysis/blob/main/Resources/RandomOverSamplerClassReport.png)

### Smote
* Balanced Accuracy - 66%
* High Risk Precision - 1%
* High Risk Sensitivity - 62%
* High Risk F1 - 2%
* Low Risk Precision - 100%
* Low Risk Sensitivity - 69%
* Low Risk f1 - 82%

![Smote](https://github.com/john10roberts/Credit_Risk_Analysis/blob/main/Resources/SmoteClassReport.png)

### ClusterCentroids
* Balanced Accuracy - 54%
* High Risk Precision - 1%
* High Risk Sensitivity - 62%
* High Risk F1 - 2%
* Low Risk Precision - 100%
* Low Risk Sensitivity - 69%
* Low Risk f1 - 82%

![Smote](https://github.com/john10roberts/Credit_Risk_Analysis/blob/main/Resources/ClusterCentroids.png)

### SMOTEENN
* Balanced Accuracy - 65%
* High Risk Precision - 1%
* High Risk Sensitivity - 72%
* High Risk F1 - 2%
* Low Risk Precision - 100%
* Low Risk Sensitivity - 58%
* Low Risk f1 - 73%

![SMOTEENN](https://github.com/john10roberts/Credit_Risk_Analysis/blob/main/Resources/SMOTEENN.png)

### BalancedRandomForestClassifier
* Balanced Accuracy - 77%
* High Risk Precision - 3%
* High Risk Sensitivity - 66%
* High Risk F1 - 6%
* Low Risk Precision - 100%
* Low Risk Sensitivity - 88%
* Low Risk f1 - 94%

![BalancedRandomForestClassifier](https://github.com/john10roberts/Credit_Risk_Analysis/blob/main/Resources/BalancedRandomForestClassifier.png)

### EasyEnsembleClassifier
* Balanced Accuracy - 92%
* High Risk Precision - 9%
* High Risk Sensitivity - 89%
* High Risk F1 - 16%
* Low Risk Precision - 100%
* Low Risk Sensitivity - 94%
* Low Risk f1 - 97%

![EasyEnsembleClassifier](https://github.com/john10roberts/Credit_Risk_Analysis/blob/main/Resources/EasyEnsembleClassifier.png)

## Summary
After evaluating each of the machine learning algorithm models, the EasyEnsemble Classifier model has the highest balanced accuracy score at 92% and a precision rank of 9% when it comes to predicting high risk customers. The low-risk sensitivity was 94% and it had a low risk f1 score of 97%. This model performed better than any of the other models and is my recommendation to use. 

The data itself might carry an implicit bias with over 99% of the eligible loans showing as low risk. This could skew the data it might make more sense to build the models on loan data from the loans charged off or paid off to see if there were ways to identify risk from this data.

