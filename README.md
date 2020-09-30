# Credit Card Fraud Detection

* This repository is for the Kaggle's Credit Card Fraud Detection to identify fraudulent credit card transactions.
* The datasets contains transactions made by credit cards in September 2013 by european cardholders.
* We did Exploratory Data Analysis, also did Data Visualization and Scaled the imbalance data because there was less number of fraudulent data then normal one.
* For handling imbalance data we evaluated the final performance of the classification models with SMOTE and random undersampling method.
* In model building we used Random Forest Classifier, Logistic Regression, Decision Tree Classifier, Support Vector Machine (SVM), K -Nearest Neighbors, Decision Tree and Gaussian Naive Bayesr.
* Also made Classification Report, defined Confusion Matrix and plotted ROC Curve.

## Resources We Used

* Jupyter Notebook.
* We used pandas, numpy, matplotlib, seaborn, imblearn (for imbalance data) and sklearn packages.
* Dataset link: https://www.kaggle.com/mlg-ulb/creditcardfraud


## Exploratory Data Analysis & Data Visualization

* We analyzed this dataset to better understand.
* Did Data Visualization in different ways with matplotlib and seaborn libraries.
* Also scaled this dataset so it can be usable for our model.


## Model Building

* First we defined the features of our scaled data then split it into test and train set with 20% test set.
* Then we used two methods to resample our data, for Oversampling we used SMOTE and for Undersampling we used Random Undersampling method.
* After scaling here we used different Models to evaluate and evaluated on the basis of recall and precision scores. (Added Accuracy and F1-Score just to show)
* With this we made Classification Report and defined Confusion Matrix for evaluation.

### SMOTE Method

**It is a type of oversampling but in this we will make the synthetic example of minority data and will give as a balanced data.** 
* In this method our Logistic Regression model has the highest Recall Score (0.928) compared to other models with poor Precision Score (0.05) from others.
* In terms of maintaining good Recall Score (0.84), Precision Score (0.91) the Random Forest Model performs better than Logistic Regression.

Model Used | Recall | Precision | Accuracy | F1-Score
------------ | ------------- | ------------- | ------------- | -------------
Random Forest Classifier | 0.84 | 0.91 | 0.99 | 0.87
Decision Tree Classifier | 0.76 | 0.45 | 0.99 | 0.57
Logistic Regression Classifier | 0.92 | 0.05 | 0.97 | 0.11
Support Vector Classifier (SVC) | 0.90 | 0.09 | 0.98 | 0.16
K-Nearest Neighbors Classifier | 0.86 | 0.48 | 0.99 | 0.61
Gaussian Naive Bayes | 0.86 | 0.06 | 0.97 | 0.11


### Undersampling Method

**It means taking the less number of majority class, in our case taking less number of normal transactions so that our new data will be balanced.**
* Random Forest performs well with excellent Recall (0.92), Precision Score (0.08) respectively.
* Followed by Logistic Regression with excellent Recall (0.92), Precision Score (0.05).

Model Used | Recall | Precision | Accuracy | F1-Score
------------ | ------------- | ------------- | ------------- | -------------
Random Forest Classifier | 0.92 | 0.08 | 0.98 | 0.14
Logistic Regression Classifier | 0.92 | 0.05 | 0.97 | 0.10
K-Nearest Neighbors Classifier | 0.90 | 0.07 | 0.97 | 0.13
Support Vector Classifier (SVC) | 0.90 | 0.06 | 0.97 | 0.11
Decision Tree Classifier | 0.90 | 0.01 | 0.91 | 0.03
Gaussian Naive Bayes | 0.86	| 0.04 | 0.96 | 0.08
