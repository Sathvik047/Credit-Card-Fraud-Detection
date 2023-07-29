# Credit-Card-Fraud-Detection

I tried to build a credit card fraud detection system using various supervised machine learning models.

## Dataset

The dataset used for this project is a credit card transaction dataset containing information about various transactions, including features derived from the transaction details and a target variable (Class) indicating whether the transaction is fraudulent (Class 1) or not (Class 0).

The dataset has the following columns:
- Time: Timestamp of the transaction
- V1-V28: Anonymized features from the original data
- Amount: Transaction amount
- Class: Target variable, 1 indicates fraud, 0 indicates legitimate transaction


## Model - 1


 **Data Preprocessing**

The dataset was extremely imbalanced, with a majority of legitimate transactions and a small number of fraudulent transactions. To address this, I performed under-sampling on the legitimate transactions to balance the dataset.

**Feature Selection**

I used the SelectKBest method with the F-statistic (f_classif) as the scoring function to select the top k features that are most relevant for the classification task.

**Supervised Machine Learning Models**

trained four different supervised machine learning models on the preprocessed data:
- Random Forest 
- XGBoost
- AdaBoost
- Logistic Regression

**Results**

The models were evaluated on the test set using various metrics


**Conclusion**

The Random Forest model achieved the highest accuracy and F1-score among the models tested. However, all models performed reasonably well in detecting credit card fraud, with high precision and recall.


