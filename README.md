\# Customer Churn Prediction using Machine Learning



\## Project Overview

This project predicts whether a customer is likely to churn using machine learning techniques. The goal is to help organisations identify at-risk customers early and improve retention strategies through data-driven insights.



\## Dataset

The dataset contains customer demographic details, service usage information, and billing features. Data preprocessing steps included:

\- Handling missing values in TotalCharges

\- Con

verting categorical variables using one-hot encoding

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

\- Confusion Matrix



\## Project Structure

