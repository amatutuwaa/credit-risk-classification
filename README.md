# credit-risk-classification

This project focuses on analyzing credit risk using machine learning models. The goal is to build a logistic regression model to predict the risk of loan default based on financial data. The analysis involves splitting the data, training the model, evaluating its performance, and writing a credit risk analysis report.


## Splitting the Data into Training and Testing Sets

To split the data in traning and testing sets I complete the following steps:
 1. Reading the lending_data.csv data from the Resources folder into a Pandas DataFrame.
 2. Creating the labels set (y) from the “loan_status” column, and then create the features (X) DataFrame from the remaining columns.
 3. Splitting the data into training and testing datasets by using `train_test_split`.


## Creating a Logistic Regression Model with the Original Data

To create a Logistic Regression Model with the Original Data I complete the following steps:

 1. Fitting a logistic regression model by using the training data (X_train and y_train).
 2. Saving the predictions for the testing data labels by using the testing feature data (X_test) and the fitted model.
 
I Evaluate the model’s performance by doing the following:
 1. Calculate the accuracy score of the model.
 2. Generate a confusion matrix.
 3. Print the classification report.

The following question was answered in the notebook: How well does the logistic regression model predict both the 0 (healthy loan) and 1 (high-risk loan) labels?


## Write a Credit Risk Analysis Report

After the analysis performed in the botebook i write a brief report that includes a summary and analysis of the performance of the machine learning models that was used in this project. This can be found in the `Credit Risk Analysis Report.md' file in the project's repo. 

