# telecom_churn

Steps Done:
1) We started with pure logistic regression using RFE. The results were abysmal as we got r2_score of approx 20% only
2) Next we tried to create a model using Random Forest. However, the grid search for optimized parameters never returned.
3) Parallely, we ran a new model using XGBoost. On the training data, the validation test data yield very good results of greater than 90%. This model we used to predict customer churn on the test data & the results were very good in the sense that it gave accuracy of 94% on the Kaggle platform.


Observations:
Based on the feature importances of XGBoost, we found the minutes of usage in the top 3 list.
Hence, we can say that good network coverage is a must as any network outage can cause customer churn.
