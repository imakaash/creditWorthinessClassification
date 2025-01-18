# Credit Worthiness Classification Project

## Overview

This project focuses on classifying credit worthiness using machine learning techniques. The analysis includes exploratory data analysis (EDA), model development, and performance evaluation.

## Contents

1.  Data Source
2.  Data Preparation
3.  Exploratory Data Analysis
4.  Model Development
5.  Feature Importance
6.  Best Credit-Worthy Profile
7.  Solution Documentation

## Data Source

The dataset was obtained from [here](https://github.com/imakaash/creditWorthinessClassification/tree/main/data), using the 'german.data' file and accompanying data dictionary.

## Data Preparation

-   Data split into train and test sets using `train_test_split` from sklearn
-   Stratification applied to ensure equal distribution of response values

## Exploratory Data Analysis

Detailed EDA, including hypothesis testing and statistical analysis, can be found in 'CreditWorthinessClassification_EDA.ipynb'.

### Sample Analysis: Number of Existing Credits

Statistical testing revealed no significant relationship between the number of existing credits and customer behavior.

## Model Development

Various models were tested, including:

-   Logistic Regression
-   K Neighbors Classifier
-   Decision Tree Classifier
-   Random Forest Classifier

Performance details are available in 'CreditWorthinessClassification_Model.ipynb'.Random Forest was chosen as the final model due to its superior performance and robustness to outliers.

## Feature Importance

Top three features according to the Random Forest model:

1.  Status of existing checking account (A11)
2.  Credit amount
3.  Duration in months

## Best Credit-Worthy Profile

A credit-worthy individual typically has:

-   Low credit amount
-   Age around 30s
-   Owns housing
-   Savings account with at least 500 DM
-   Purpose not related to used car, business, education
-   No guarantors/debtors
-   Some property ownership
-   No other installment plans

## Solution Documentation

### Code

-   EDA: 'CreditWorthinessClassification_EDA.ipynb'
-   Model: 'CreditWorthinessClassification_Model.ipynb'

### Model Performance

Performance evaluated using:

-   F1 score
-   Recall
-   KS decile coverage
-   ROC AUC score

### Visualizations

-   Lift chart
-   Cumulative gain chart
-   KS chart
-   ROC AUC curve
