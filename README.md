# Customer-Churn-Prediction-Churn-Analysis-of-a-Telecom-Company

ML Model that has been developed in this repository is expected to output a `Churn Probability` for every data under test. 
The input data is spread over 3 separate files - `churn_data.csv`, `cust_data.csv` and `internet_data.csv`. 

The Data includes the following: 

- `Personal Data (gender, children, whether senior citizen, dependents...)`
- `Services Related (Tenure with the provider, payment method, internet packs purchased, special offers...)`
- `Charges being incurred (Amount of recharge done per month...)`

Following steps are covered in the code:

1. Importing three datasets and merging them on 'CustomerID'
2. Feature Engg
3. Univariate Analysis:
	I.   Churn Split in terms of Counts
	II.  Find for which kind of Contracts the churn probability is more
	III. Whether being on Monthly Charges is influencing Churn
	IV.  Whether TotalCharges amount has influence on Churn
	V.   Whether having Multiple Internet Connections have influence on Churn
	VI.  Whether type of Internet Service has influence on Churn
	VII. 
4. Encoding of cetegorical features
5. Handling Missing values
6. Train Test Split
7. Feature Scaling
8. Finding co-relation between features and dropping highly corelated features
9. Create optimised Logistic Regression Model using Statsmodel Logit()
10. Feature Selection: Drop Features with P-Value > 0.05
11. Recreate the Logit Model with updated set of columns
12. Create optimised Logistic Regression Model using ScikitLearn
13. Predict using Training Data
14. Calculate Classification Metrics (Sensitivity/Recall, Specificity, Precision)
15. Plot ROC Curve and AUC
16. Finding optical threshold point (Cutoff point for separating class 0 and class 1) using Plot of 'accuracy - sensitivity - specificity' against various probabilities.
17. Recalculate Precision and Recall 
18. Plotting the Precision-Recall Curve and find Precision-Recall tradeoff
19. Making predictions on the Test Data
