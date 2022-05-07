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
- Balanced accuracy score: 0.6463970560994359
- Precision and Recall can be found in the pre and rec columns below:
![Oversampling with RandomOverSampler](/Images/RandomOverSampler_classificationReport.PNG)

#### SMOTE Oversampling
- Balanced accuracy score: 0.6586230769943224
- Precision and Recall can be found in the pre and rec columns below:
![Oversampling with SMOTE](/Images/SMOTE_classificationReport.PNG)

#### ClusterCentroids Undersampling
- Balanced accuracy score: 0.5442369453268994
- Precision and Recall can be found in the pre and rec columns below:
![Undersampling with ClusterCentroids](/Images/ClusterCentroids_classificationReport.PNG)

#### SMOTEENN Combination Sampling
- Balanced accuracy score: 0.6664711051320287
- Precision and Recall can be found in the pre and rec columns below:
![Combination Sampling with SMOTEENN](/Images/SMOTEENN_classificationReport.PNG)

#### BalancedRandomForestClassifier Ensemble Learning
- Balanced accuracy score: 0.8735251380412671
- Precision and Recall can be found in the pre and rec columns below:
![Ensemble Learning with BalancedRandomForestClassifier](/Images/BalancedRandomForestClassifier_classificationReport.PNG)

#### EasyEnsembleClassifier Ensemble Learning
- Balanced accuracy score: 0.9154459266085636
- Precision and Recall can be found in the pre and rec columns below:
![Ensemble Learning with EasyEnsembleClassifier](/Images/EasyEnsembleClassifier_classificationReport.PNG)

In viewing the results above, the following can be concluded:

- Naive Random Oversampling makes the correct predictions about 65% of the time, identifies 1% of the actual high-risk candidates, and incorrectly labels low-risk candidates as high-risk 58% of the time. 

- SMOTE Oversampling makes the correct predictions about 66% of the time, identifies 1% of the actual high-risk candidates, and incorrectly labels low-risk candidates as high-risk 68% of the time. 

- ClusterCentroids Undersampling makes the correct predictions about 54% of the time, identifies 1% of the actual high-risk candidates, and incorrectly labels low-risk candidates as high-risk 40% of the time. 

- SMOTEENN Combination Sampling makes the correct predictions about 67% of the time, identifies 1% of the actual high-risk candidates, and incorrectly labels low-risk candidates as high-risk 60% of the time. 

- BalancedRandomForestClassifier Ensemble Learning makes the correct predictions about 87% of the time, identifies 3% of the actual high-risk candidates, and incorrectly labels low-risk candidates as high-risk 87% of the time. 

- EasyEnsembleClassifier Ensemble Learning makes the correct predictions about 92% of the time, identifies 5% of the actual high-risk candidates, and incorrectly labels low-risk candidates as high-risk 90% of the time. 

## Summary

In summary, I would not recommend any of the models. Although there were some models with incredibly high accuracy scores, all models had low precision for high-risk candidates, meaning that most of the high-risk candidates slipped thru the cracks and were not labeled as high-risk, allowing them to get approved for loans. Additionally, many of the models had high recall scores for low-risk candidates, meaning that many low-risk candidates were labeled as high-risk, and would be denied a loan. 
