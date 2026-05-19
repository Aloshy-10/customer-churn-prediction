\# Customer Churn Prediction using Machine Learning



\## Project Overview

This project predicts whether a customer is likely to churn using machine learning techniques. The goal is to help organisations identify at-risk customers early and improve retention strategies through data-driven insights.



\## Dataset

The dataset contains customer demographic details, service usage information, and billing features. Data preprocessing steps included:

\- Handling missing values in TotalCharges

\- Converting categorical variables using one-hot encoding


\- Removing unnecessary columns such as customerID



\## Models Used

The following machine learning models were implemented and evaluated:

\- Logistic Regression

\- Random Forest Classifier

\- XGBoost Classifier



\## Handling Class Imbalance

The dataset contained imbalanced target classes. This was addressed using:

\- scale\_pos\_weight in XGBoost



\## Evaluation Metrics

Model performance was evaluated using:

\- Accuracy

\- Precision

\- Recall

\- F1-score

\- Confusion_matrix


----
## Why scale_pos_weight is used?


It is because dataset is imbalanced, which means more customer stayed and few customers churned
Here model sees way more "not churn" example
---
## Problem without scale_pos_weight

If we train model without scale_pos_weight the model thinks most customer didn't churn so it will predict NOT churn for everyone
Then we get high accuracy but bad churn detection
---
## Why is it dangerous

In real business missing a churn customer= losing revenue, so detecting chur customer is very important
---
## What scale_pos_weight does?

It tell the model to pay more attention to churn customers





