# Module 20 Report: Credit Risk Logistic Regression Model

## Overview of the Analysis

The purpose of this analysis is to create a supervised machine learning model that can predict the status of a potential loan as *healthy* or *high-risk*. The following features were used as input variables to develop the model:

* **Loan Size**
* **Interest Rate**
* **Borrower Income**
* **Debt to Income Ratio**
* **Number of Accounts**
* **Derogatory Marks**
* **Total Debt**

Additionally, **Loan Status**, a binary variable, was used as the output variable. The following steps were taken to develop and train the model:

* The input and output features were split into training and testing data using `train_test_split`.
* The input training and testing data sets were scaled using `StandardScaler`.
* A logistic regression model was instantiated using `LogisticRegression` with a solver of `lbfgs` and 200 max iterations.
* The training data was fitted to the logistic regression model.
* The model was used to make predictions based on the testing input data.
* The predictions were compared to the testing output data utilizing a confusion matrix and a classification report.

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

