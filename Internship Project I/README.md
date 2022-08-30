## Overview of Project
In this project the task was to predict correctly whether a person is suffering from Parkinson's disease or not and the major objective was to get a "False Neagtive Rate"
0.1

This is a binary classification task and the focus is on increasing the "Recall". Hence, the metric used is "F2 score".
An important insight regarding data is that, it is an imbalanced data, so I have used the "Oversampling" technique which gives good model performance.

## Data Manipulation
1. No null values.
2. Applying Box-cox transformation to reduce the number of outliers.
3. Median imputation for remaining outliers.
4. Dropping highly correlated features.
5. Using Oversampling.

## Models used (with hyperparametre tuning):
1. Random Forest 
2. Light Gradient Boosting Classifier.

## Model Evaluation
1. Apply calibration on top of the model to get probability scores.
2. Get True positive rate & False positive rate through auc_score.
3. Using the TPR & FPR values to get the best threshold with "Youden J statistic".
4. Defining a custom function to get the False negative rate with the best threshold.

## Results
1. Random Forest - False Negative Rate : 0.068
2. LGB Classifier - False Negative Rate :0.06818
