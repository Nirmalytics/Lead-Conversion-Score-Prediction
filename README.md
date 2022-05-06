# Lead-Conversion-Score-Prediction
Predicting the customers that would show more intent towards a recommended credit card

## PREDICTION MODEL
I created an XGBClassifier model with parameters, 

{learning_rate =0.1,
 n_estimators=100,
 max_depth=5,
 min_child_weight=1,
 gamma=0.15,
 subsample=0.8,
 colsample_bytree=0.8,
 objective= 'binary:logistic',
 nthread=4,
 scale_pos_weight=1,
 seed=101} which give a Roc_Auc score of 0.8715286129

## Conclusion
Age have a role on Creditcard interest.
As age increase, CreditcardInterest also increase.
Those customers with high 'Vinate_Age_ratio' will have more chance of conversion
Customers who had availed earlier Credit_Products and those customers who are reluctant to answer had more chance for Lead conversion
Saalaried and Other occupation has more chance for leadConversion

