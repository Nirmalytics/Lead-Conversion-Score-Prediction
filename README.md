#Credit Card Lead-Conversion-Score-Prediction

## Problem Statement

Happy Customer Bank is a mid-sized private bank that deals in all kinds of banking products, like Savings accounts, Current accounts, investment products, credit products, among other offerings. The bank also cross-sells products to its existing customers and to do so they use different kinds of communication like tele-calling, e-mails, recommendations on net banking, mobile banking, etc. In this case, the Happy Customer Bank wants to cross sell its credit cards to its existing customers. The bank has identified a set of customers that are eligible for taking these credit cards.
Now, the bank is looking for your help in identifying customers that could show higher intent towards a recommended credit card, given:

Customer details (gender, age, region etc.) 

Details of his/her relationship with the bank (Channel_Code,Vintage, 'Avg_Asset_Value etc.)

## Predict the customers that could show higher intent towards a recommended credit card

### expected inputs to the model

Customer details (gender, age, region etc.)

Details of his/her relationship with the bank (Channel_Code,Vintage, Avg_Asset_Value etc.)

Target variable : Is_Lead (Lead_Prediction)

evaluation protocol -The evaluation metric for this Problem is roc_auc_score

Its a Supervised - classification problem

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

