# Module 20 Report: Credit Risk Logistic Regression Model

![image](https://github.com/lvit001/credit-risk-classification/assets/140283164/a3d7e75b-b727-4423-8737-4b093413aab4) [Image Source](https://www.google.com/url?sa=i&url=https%3A%2F%2Fburgosandbrein.com%2FFactors-and-How-to-Avoid-Them-3564442.html&psig=AOvVaw2B-rO60fph4Pk8A92Q3elk&ust=1709416737061000&source=images&cd=vfe&opi=89978449&ved=0CBMQjRxqFwoTCJjlid2H1IQDFQAAAAAdAAAAABAE)

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

* [x] The input and output features were split into training and testing data using `train_test_split`.
* [x] The input training and testing data sets were scaled using `StandardScaler`.
* [x] A logistic regression model was instantiated using `LogisticRegression` with a solver of `lbfgs` and 200 max iterations.
* [x] The training data was fitted to the logistic regression model.
* [x] The model was used to make predictions based on the testing input data.
* [x] The predictions were compared to the testing output data utilizing a confusion matrix and a classification report.

## Results

* **Logistic Regression Model Performance:**
  * The model had an accuracy score of **99%**
  * **Healthy Loan Predictions**
    * **Precision:** _100%_
    * **Recall:** _100%_
  * **High-Rish Loan Predictions**
    * **Precision:** _87%_
    * **Recall:** _98%_

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

