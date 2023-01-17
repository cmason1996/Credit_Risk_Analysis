# Credit_Risk_Analysis

## Overview

The purpose of this project was to run an analysis on the risk for credit lenders for individuals seaking loans or lines of credit based on supplied factors. To do this we used various different sampling techniques as well as Linear Regression and Random Forest models to determine the best model to observe and then make predictions about the data.

Tools Used:
* Jupyter Notebook ipyKernel version 6.9.1
* Python version 3.9.12
* Data from LoanStats_2019Q1.csv

## Results

<a href="https://github.com/cmason1996/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb" target="_blank">Click here to view the code for Over and Undersampling</a>

### Oversampling

#### Niave Random Oversampling

<img width="516" alt="niave_oversampling" src="https://user-images.githubusercontent.com/112291888/212794647-d4a0cad2-dfd9-4b34-a1d5-5da817dfc32a.png">

With an average accuracy of 67.14%, a precision of .99, and a recall of .67; 

#### SMOTE Oversampling

<img width="518" alt="SMOTE_oversampling" src="https://user-images.githubusercontent.com/112291888/212794659-7d247cc8-5eed-4592-bf05-e83245b9a993.png">

With an average accuracy of 65.79%, a precision of .99, and a recall of .66; 

* Oversampling appears to be the middle ground here, neither highly inaccurate or highly accurate. Given the choice, other models may be better for the prediction of credit risk, but should speed be the necessary qualification, this method in combination with the Linear Regression model will return a relatively accurate prediction on the risk level of loan seekers.

### Undersampling

#### Cluster Centroid Undersampling

INSERT CLUSTER SAMPLING HERE

With an average accuracy of 45.02%, a precision of .99, and a recall of .45;

* This is the least accurate of all the models tried for this analysis and we would not recommend further use of it as it failed to correctly identify all of the true positives for the low and high-risk categories.

### Combination Over and Undersampling

INSERT SMOTEET HERE

With an average accuracy of 53.49%, a precision of .99, and a recall of .53; 

### Random Forest

<a href="https://github.com/cmason1996/Credit_Risk_Analysis/blob/main/credit_risk_ensemble.ipynb" target="_blank">Click here to view the Random Forest Code</a>

INSERT FOREST HERE

With an average accuracy of 90.76%, a precision of .99, and a recall of .91;

* This model is one of the more accurate that we used and this is most likely due to the many number of different instances that were called to make predictions, in this case 100 different trees, which checked the mistakes of others and created an accurate and reliable model. 

### Easy AdaBoost

INSERT ADABOOST HERE

With an average accuracy of 94.28%, a precision of .99, and a recall of .94; 

* This is the most accurate of all of the different models we tried and is the model that we would recommend for further analysis of the data or to predict results to credit-lenders.

## Summary

### Findings

Overall the Easy Ensenble AdaBoost Classifier is the most accurate learning model for this analysis as it correctly identifies the highest number of true positives and true negatives out of all of the models while maintaining precision and increasing accuracy.

### Recommendations

Going forward with this analysis, it is recommended to attempt to replicate all of the results from all of the various models tested to ensure that the results gained from them are true and accurate. In addition, it is also recommended to run an analysis with the Easy AdaBoost model on a different set of credit records and then generate an accuracy score and confusion matrix to ensure that this learning model can be generalized to other datasets. 
