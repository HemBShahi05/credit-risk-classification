Credit Risk Classification (Supervised Machine Learning Model)

Overview of the Analysis

1.The analysis aimed to build a supervised machine learning model that could predict the creditworthiness of borrowers using historical lending data from a peer-to-peer lending service.
2.The dataset included information on the loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, and derogatory marks, while the dependent variable was the loan status, indicating whether a loan was healthy or at risk.
3.The analysis involved splitting the data into training and test sets, defining the dependent and independent variables, creating a logistic regression model, fitting the original data to the model, and making predictions based on the trained model. 
4.Two different logistic regression models were created, one using the original dataset and another using a randomly oversampled dataset to address the imbalances in the data.

Results
1.Logistic Regression Model with Original Data

       Balanced Accuracy Score: 0.940636519048405

                precision    recall  f1-score   support

           0       1.00      1.00      1.00     18748
           1       0.88      0.89      0.88       636

    accuracy                           0.99     19384
   macro avg       0.94      0.94      0.94     19384
weighted avg       0.99      0.99      0.99     19384

                
2.  Logistic Regression Model with Randomly Oversampled Data

       Balanced Accuracy Score: 0.9914437833536626     


                precision    recall  f1-score   support

           0       1.00      1.00      1.00     18748
           1       0.88      0.99      0.93       636

    accuracy                           1.00     19384
   macro avg       0.94      0.99      0.96     19384
weighted avg       1.00      1.00      1.00     19384







Summary
The results showed that the collected data could effectively train and test a machine learning classification model. However, the model's performance could be improved by addressing the imbalances in the data. Randomly oversampling the data led to higher balanced accuracy and recall scores, allowing the model to more accurately predict risky loans.

In terms of incorrect predictions, false positives and false negatives both have costs, and it's important for the model to have good accuracy in predicting both. The summary also noted that potential ways to improve the model's performance include using different machine learning algorithms, feature engineering, or hyperparameter tuning.

Overall, the analysis demonstrated the potential of supervised machine learning models to predict credit risk and highlighted the importance of addressing imbalances in the data for accurate predictions.
