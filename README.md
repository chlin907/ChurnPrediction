



# Telecommunication Churn Prediction

In this project, we use supervised learning models to identify customers who are likely to stop using telecommunication service in the future. Furthermore, we will analyze top factors that influence user retention from model itself. The dataset source is <https://www.kaggle.com/pangkw/telco-churn/home>

## Model Performance

Performance across vairous model is summarized below. The eXtreme Gradient Boosting (XGBOOST) obvisouly outperform others in every aspect. 

| Model Name                  | CV Accuracy | Precision | Recall   | F1 score |
| --------------------------- | ----------- | --------- | -------- | -------- |
| Logistic regression with L1 | 0.893029    | 0.690691  | 0.476190 | 0.563725 |
| Logistic regression with L2 | 0.893029    | 0.686217  | 0.484472 | 0.567961 |
| Random forest               | 0.913161    | 0.854015  | 0.484472 | 0.618230 |
| KNN                         | 0.893029    | 0.757085  | 0.387164 | 0.512329 |
| SVM                         | 0.916767    | 0.836601  | 0.530021 | 0.648923 |
| XGBOOST                     | 0.947716    | 0.885287  | 0.734990 | 0.803167 |
| XGBOOST optimized           | 0.956130    | 0.933162  | 0.751553 | 0.832569 |



## What else does a predictive model tell us?

From the businees point of view, what is more critical is that the top factors we can extract from our trained model? If we list all features by their feature importance, The top five predictive features are TotalDayMinutes, TotalEveMinutes, TotalIntlMinutes, CustomerServiceCalls and TotalNightMinutes. Four out of them are related to the call usage. Conclusively, we may suggest that the company may provide a discount plan for heavy users and investigate the customer service call quality.

![screenshot](/Users/chiahuilin/work/project/Churn_prediction/misc/screenshot.png)









