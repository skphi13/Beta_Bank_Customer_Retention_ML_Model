# Beta_Bank_Customer_Retention_ML_Model
Beta Bank customers are leaving, chipping away at the bank little by little every month. We need to predict whether a customer will leave soon.

## Goal
Build a model with the maximum possible F1 score. Additionally, measure the AUC-ROC metric and compare it with the F1.

## Data Description

 Features

- RowNumber — data string index
- CustomerId — unique customer identifier
- Surname — surname
- CreditScore — credit score
- Geography — country of residence
- Gender — gender
- Age — age
- Tenure — period of maturation for a customer’s fixed deposit (years)
- Balance — account balance
- NumOfProducts — number of banking products used by the customer
- HasCrCard — customer has a credit card
- IsActiveMember — customer’s activeness
- EstimatedSalary — estimated salary

 Target

- Exited — сustomer has left

## Conclusion
For this project we completed the following:

   Data Preperation:
   - Handled missing values in the `Tenure` column.
   - Looked at distribution of quantitative columns.

    
   Model Creation:
   - Encoding completed since strings were present in our features
   - Split the data into features and target. Our target column was the `Exited` column since we were identifying customers who left.
   - After transforming the features we continued onto scaling them to standardize them.
   
   Final Model Test:
   - The Random Forest had our highest F1 score so we used this model for our final model test.
   - F1 score: 62%
   - Accuracy: 85%
   - AUC-ROC: 86%
      
      
Conclusion:

The Random Forest model seems to be the best in predicting whether customers stay or not with Beta Bank. This most creates a significan number of True Negatives (0), this shows that many customers are likely to stay.
