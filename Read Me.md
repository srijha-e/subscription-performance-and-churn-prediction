**Subscription Customer Churn using LightGBM**

This project aims to identify customer churn using LightGBM, an efficient gradient boosting algorithm. The goal is to identify customers who are likely to cancel their subscriptions so proper steps can be taken to retain them. 

**About Dataset:**  
The dataset used is the Customer Subscription Data from Kaggle. This dataset contains information related to a subscription-based digital product offering financial advisory that includes newsletters, webinars, and investment recommendations.   
The data set contains the following information:

1. Customer sign-up and cancellation dates  
2. Call center activity  
3. Customer demographics  
4. Product pricing info

**Workflow**:

1. Exploratory Data Analysis (EDA)  
2. Data Preprocessing & Class Balancing  
3. LightGBM Model Implementation  
4. Model Evaluation  
5. Feature Importance Analysis

**Exploratory Data Analysis:**  
As a part of EDA we cover following aspects:

1. Data Cleaning  
2. Data Distribution   
   1. Customer Demographics  
   2. Trend Analysis   
   3. Channel Distribution  
   4. Reason Analysis  
   5. Subscriptions vs Cancellation Distribution.  
3. Feature Correlations

These insights helped in understanding behavior patterns and identifying the most influential predictors of churn.

**Data Preprocessing:**

1. Encoding categorical variables  
2. Converted date fields into useful features  
3. Added new features  
4. Handled class imbalance using SMOTE to prevent overfitting. 

**Model Implementation and Evaluation:**  
Implemented LightGBM model due to its ability to handle large datasets and strong performance for classification tasks.  
Applied hyperparameter tuning with RandomizedSearchCV and used the optimal parameters to fit the final LightGBM model.
The model is evaluated on the test set evaluated using Accuracy, Precision, Recall, F1-score, ROC-AUC and Confusion Matrix.  
Identified feature importance and eliminated less important features.

The model achieved:  
Test Accuracy: \~0.84  
Cross-Validation Accuracy: \~0.77  
Good precision for non-churn class and balanced precision–recall for churned class.

**Conclusion:**  
The difference between test accuracy and cross-validation accuracy indicates that the model performs reasonably well on new, unseen data and is not heavily overfitting.  
The model can be further improved with Hyperparameter tuning, trying additional algorithms and adding more domain-specific features
