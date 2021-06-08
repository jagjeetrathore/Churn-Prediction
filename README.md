# Churn Prediction
## Objective:



**Churn**
* Cancellation of Subscription
* Closure of an active account
* End of relationship between Subscriber and provider
 
**Hypothesis:**
 
* Supervised Classification Problem
* Predict that the customer will churn or not look at historical data.Try to find associated probabilities.
* How can Talcum reduce the churn ratio so that telecom company stay in business
 
**Preprocessing**
 
* Find Missing values
* how features are  interrelated or correlated.
* Perform descriptive analysis to find the datatype of each feature.
* Find mean, min and mix of numerical features
* Find Count, frequency of categorical features
* Customer satisfaction is hardest to capture since it does not have features   like product rating or customer support calls.
 
**Exploratory Data Analysis**
 
**Feature Engineering**
 
* Convert numerical features like Total Charges,Monthly charges in to segments using K-means clustering, so that those segments can be easily communicated to business people
* used panadas get_dummies function and label encoder  to handle categorical features.
 
**Predictive Modelling**
* Handling imbalanced dataset with  various SMOTE (oversampling and undersampling Techniques) Techniques were applied on various machine learning model like Logistic Regression, Decision Tree and RandomForest 
 
`SMOTE is an oversampling method that balances imbalanced datasets by sampling (with replacement) minority class.` SMOTE-NC stands for Synthetic Minority Over-sampling TEchnique for data with Numerical-Categorical features. Note that only training data is oversampled. The testing data is untouched.

**Hyperparameter Tuning*
 
max_depth controls the depth of the tree in Random Forest.
Change the number of variables that are sampled at each split. 
use AUC as comparison metric
 
**Best Model** 
 
 (RandomForest)
One of the advantages of Random Forest was it can work with highly correlated features. It can deal with non-linearities much better than logistic Regression.
To make predictions it uses multiple decision trees which is more effective than a single decision tree.
Then for each observation that it encounters from each node, it chooses their category by taking the majority vote of different trees.
6.The data with low bias & high variance (non-linear relationships) can be handled properly & efficiently.
 
 
**Model Evaluation**
 
Evaluate the various models like LogisticRegression, DecisionTree, RandomForest using Recall (sensitivity)  as a metric.
sensitivity is a measure of how well a model can identify true positives.
sensitivity is...............................
That means with this model we can predict 74% of time who will Churn beforehand with current features.
let us Look at **AUC** which is ........ which is much better than our baseline model .........
 
**References**
 
* One of the advantages of Random Forest was it can work with highly correlated features. It can deal with non-linearities much better than logistic Regression.
To make predictions it uses multiple decision trees which is more effective than a single decision tree.
Then for each observation that it encounters from each node, it chooses their category by taking the majority vote of different trees.
`The data with low bias & high variance (non-linear relationships) can be handled properly & efficiently.`


**Model Evaluation**
The 3 model were evaluated with Recall metric.
![image](https://user-images.githubusercontent.com/47728397/116484517-3c2aef80-a857-11eb-8062-26b69f6a14a5.png)


![image](https://user-images.githubusercontent.com/47728397/116484333-dcccdf80-a856-11eb-8414-005a5b77a94b.png)

