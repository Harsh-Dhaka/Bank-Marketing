# Bank-Marketing:
* There has been a revenue decline for the Portuguese bank and they would like to know what actions to take. After investigation, they found out that the root cause is that their clients are not depositing as frequently as before. Knowing that term deposits allow banks to hold onto a deposit for a specific amount of time, so banks can invest in higher gain financial products to make a profit. In addition, banks also hold better chance to persuade term deposit clients into buying other products such as funds or insurance to further increase their revenues. As a result, the Portuguese bank would like to identify existing clients that have higher chance to subscribe for a term deposit and focus marketing effort on such clients.

* To resolve the problem, we suggest a classification approach to predict which clients are more likely to subscribe for term deposits.

# Attribute Information:
* The data is related with direct marketing campaigns of a Portuguese banking institution. 
* The marketing campaigns were based on phone calls. Often, more than one contact to the same client was required,in order to access if the product (bank term deposit) would be (or not) subscribed. The classification goal is to predict if the client will subscribe a term deposit (variable y).
* The dataset contains 45211 rows and 17 columns

# Data Preprocessing and EDA:
* While checking for the missing values we see there are 0 missing values shown in the dataset because there are several missing values in some categorical attributes, all coded with the "unknown" label.(Variables like job,education,contact_via,poutcome contains unknown values.) 
* These missing values can be treated as a possible class label or using deletion or imputation techniques.
* By looking at percentage values in target variable we infer that data is imbalanced.
* Performed some feature engineering and used some user defined functions for some of the variables.
* Used different types of plots to visualize the data in a better way(Barplot,scatterplot,pairplot).
* Checked for multicollinearity using VIF as the data is imbalanced.
* Performed some of the statistical tests to check the relation of variables with target variable and among each other also.(Chi-Square test of Independence,Anova)
* Encoded categorical variables and scaled numerical variables for the further modelling.
* To deal with the problem of imbalancing in the data we used SMOTE technique to balance the data.
* After splitting the data using train_test_split.

# Model:
* We consider Logistic Regression as our base model.
* Then we used ROC_AUC curve for checking the obtained result.
* After LG we used cross validation technique from which got a roc_auc score around 0.86.
* Used KNN Classifier,Random Forest and boosting technique Adaboost,Gradient Boosting. 


