**Subscription Performance and Churn using LightGBM
**
This project aims to identify customer churn using LightGBM, an efficient gradient boosting algorithm. The goal is to identify customers who are likely to cancel their subscriptions so proper steps can be taken to retain them. 

**About Dataset:
**
The dataset used is the Customer Subscription Data from Kaggle. This dataset contains information related to a subscription-based digital product offering financial advisory that includes newsletters, webinars, and investment recommendations. 
The data set contains the following information:
Customer sign-up and cancellation dates
Call center activity
Customer demographics
Product pricing info

Workflow:
Exploratory Data Analysis (EDA)
Data Preprocessing & Class Balancing
LightGBM Model Implementation
Model Evaluation
Feature Importance Analysis

Exploratory Data Analysis:
As a part of EDA we cover following aspects:
Data Cleaning
Data Distribution 
Customer Demographics
Trend Analysis 
Channel Distribution
Reason Analysis
Subscriptions vs Cancellation Distribution.
Feature Correlations
These insights helped in understanding behavior patterns and identifying the most influential predictors of churn.

Data Preprocessing:
Encoding categorical variables
Converted date fields into useful features
Added new features
Handled class imbalance using SMOTE to prevent overfitting. 

Model Implementation and Evaluation:
Implemented LightGBM model due to its ability to handle large datasets and strong performance for classification tasks.
The model is evaluated on the test set evaluated using Accuracy, Precision, Recall, F1-score, ROC-AUC and Confusion Matrix.
Identified feature importance and eliminated less important features.

The model achieved:
Test Accuracy: ~0.84
Cross-Validation Accuracy: ~0.77
Good precision for non-churn class and balanced precision–recall for churned class.

Conclusion:
The difference between test accuracy and cross-validation accuracy indicates that the model performs reasonably well on new, unseen data and is not heavily overfitting.
The model can be further improved with Hyperparameter tuning, trying additional algorithms and adding more domain-specific features.
