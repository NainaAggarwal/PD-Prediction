# PD-Prediction
Develop a data-driven credit risk model to predict the probabilities of default (PD) 

Steps followed:
1.	Observed the dataset by determining the size including number of rows and columns the dataset holds.
2.	Understand the variables that will help in making decisions.
3.	Categories the variables into continuous, discrete and categorical and visualise the data. Check if there is outliers or skewness in the variables that helps to understand the data better. 
4.	Looked for the missing values in the dataset and what cause them missing. Is it missing at random or missing not at random.
5.	Used StandardScaler for feature Scaling
6.	Used Resampling Technique to handle imbalance Data
7.	Build the following models to predict PD
    a. Logistic Regression
    b. Random Forest
    c. XGBoost
8. Used Train-test split and cross validation technique to validate data
9. Evaluated the models on below metrics and select the best performer:
    •	ROC of all the models
    •	Confusion metrics  
    •	Train & Test Accuracy
    •	Precision
    •	Recall
    •	F1 score
10: Determine the top most important predictor variables in the models


Two primary ways used to handle the missing values:  
1.	Deleting the missing values
2.	Imputing the missing values

Deleting the missing values -  Either by deleting the entire row or by deleting the columns that has less relevance in data analysis. Eg:  If a column holds a lot of missing values, say more than 80%, and the feature is not meaningful, then I have dropped the entire column. 

Imputing the missing values:
1.	Imputation with constant value : replaces the missing values with either zero or any constant value.
2.	Imputation using Statistics: Before using any statistics technique, first check the type of data and distribution of features(if numeric). Accordingly  can impute the missing values with either “Mean” or “Median” or “Mode”. Mean is preferred if data is numeric and not skewed. Median is preferred if data is numeric and skewed. Mode is preferred if data is a string(object) or discrete.
3.	Advanced imputation techniques – Using KNN imputer (by finding the closest neighbors) or by using Weight of evidence (WOE) – by creating binning.

Ways to detect outliers
1.	Creating the box plot/ scatter plot to detect univariate outliers or multivariable outliers.
2.	Histogram is also used to detect the outliers in the data distribution of a single variable
3.	For normal distributions, use empirical relations of Normal distribution. The data points that falls fall below mean-3*(sigma) or above mean+3*(sigma) are outliers.





