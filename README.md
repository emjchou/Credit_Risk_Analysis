# Credit_Risk_Analysis

## Overview of analysis

The purpose of this analysis is to use Ensemble Learning and different Sampling techniques to deal with doing machine learning on an unbalanced loan dataset, in order to predict credit risk. 

## Results

Balanced accuracy score is the ratio of correct predictions to total predictions.

Precision score is a measure of how reliable a positive classification is, represented by a ratio of true positive values to the number of all positives.

Recall, or Sensitivity, is a ratio of true positive outcomes to actually true outcomes. 

In the case of credit risk analysis, Accuracy will represent a measure of how often the model makes correct predictions, Precision for high_risk will represent how often a predicted high risk candidate is actually high risk, and Recall for high_risk will represent how often an actual high risk candidate is labeled as high risk. With these definitions in mind, the following classification reports (containing precision and recall) and accuracy scores can be examined. 

### Classification Reports

#### Naive Random Oversampling (RandomOverSampler model)
Balanced accuracy score: 0.6463970560994359
Precision for high_risk: 0.01
Recall for high_risk: 0.71
![Oversampling with RandomOverSampler](/Images/RandomOverSampler_classificationReport.PNG)

#### SMOTE Oversampling
Balanced accuracy score: 0.6586230769943224
Precision for high_risk: 0.01
Recall for high_risk: 0.63
![Oversampling with SMOTE](/Images/SMOTE_classificationReport.PNG)

#### ClusterCentroids Undersampling
Balanced accuracy score: 0.5442369453268994
Precision for high_risk: 0.01
Recall for high_risk: 0.69
![Undersampling with ClusterCentroids](/Images/ClusterCentroids_classificationReport.PNG)

#### SMOTEENN Combination Sampling
Balanced accuracy score: 0.6664711051320287
Precision for high_risk: 0.01
Recall for high_risk: 0.73
![Combination Sampling with SMOTEENN](/Images/SMOTEENN_classificationReport.PNG)

#### BalancedRandomForestClassifier Ensemble Learning
Balanced accuracy score: 0.8735251380412671
Precision for high_risk: 0.03
Recall for high_risk: 0.70
![Ensemble Learning with BalancedRandomForestClassifier](/Images/BalancedRandomForestClassifier_classificationReport.PNG)

#### EasyEnsembleClassifier Ensemble Learning
Balanced accuracy score: 0.9154459266085636
Precision for high_risk: 0.05
Recall for high_risk: 0.93
![Ensemble Learning with EasyEnsembleClassifier](/Images/EasyEnsembleClassifier_classificationReport.PNG)


, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.