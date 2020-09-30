# Credit Card Fraud Detection

* This repository is for the Kaggle's Credit Card Fraud Detection to identify fraudulent credit card transactions.
* The datasets contains transactions made by credit cards in September 2013 by european cardholders.
* We did Exploratory Data Analysis and Scaled the imbalance data because there was less number of fraudulent data then normal one.
* For handling imbalance data we evaluated the final performance of the classification models with SMOTE and random undersampling method.
* In model building we used Random Forest Classifier, Logistic Regression, Decision Tree Classifier, Support Vector Machine (SVM), K -Nearest Neighbors, Decision Tree and Gaussian Naive Bayesr.

## Resources We Used

* Jupyter Notebook.
* We used pandas, numpy, sklearn, matplotlib, seaborn packages.
* Dataset link: https://www.kaggle.com/c/titanic/overview


## Data Cleaning and Exploratory Data Analysis

* We analyzed and cleaned this dataset so it can be usable for our model
* And in EDA part, we simplified our data and analyzed different value counts through graphs also through pivot table


## Model Building

* We transformed our variables into dummy variables
* Here we used different Models to evaluate
* The Random Forest model performed better than the other approaches on the test set. 

Model Used| Score
------------ | -------------
Random Forest | 94.84%
Decision Tree	 | 94.84%
Voting Classifier	 | 88.66%
K -Nearest Neighbors	 | 87.32%
Logistic Regression	 | 84.62%
Support Vector Machine (SVM)	 | 76.21%
Gaussian Naive Bayes	 | 75.31%


