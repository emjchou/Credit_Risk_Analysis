# Credit_Risk_Analysis

## Overview of analysis

The purpose of this analysis is to use Ensemble Learning and different Sampling techniques to deal with doing machine learning on an unbalanced loan dataset, in order to predict credit risk. 

## Results

### Classification Reports

Naive Random Oversampling (RandomOverSampler model)
Balanced accuracy score: 0.6463970560994359
![Oversampling with RandomOverSampler](/Images/RandomOverSampler_classificationReport.PNG)

SMOTE Oversampling
Balanced accuracy score: 0.6586230769943224
![Oversampling with SMOTE](/Images/SMOTE_classificationReport.PNG)

ClusterCentroids Undersampling
Balanced accuracy score: 0.5442369453268994
![Undersampling with ClusterCentroids](/Images/ClusterCentroids_classificationReport.PNG)

SMOTEENN Combination Sampling
Balanced accuracy score: 0.6664711051320287
![Combination Sampling with SMOTEENN](/Images/SMOTEEN_classificationReport.PNG)

BalancedRandomForestClassifier Ensemble Learning
Balanced accuracy score: 0.8735251380412671
![Ensemble Learning with BalancedRandomForestClassifier](/Images/BalancedRandomForestClassifier_classificationReport.PNG)

EasyEnsembleClassifier Ensemble Learning
Balanced accuracy score: 0.9154459266085636
![Ensemble Learning with EasyEnsembleClassifier](/Images/EasyEnsembleClassifier_classificationReport.PNG)


, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.