# Module 20 Report: Credit Risk Logistic Regression Model

![image](https://github.com/lvit001/credit-risk-classification/assets/140283164/a3d7e75b-b727-4423-8737-4b093413aab4) [Image Source](https://www.google.com/url?sa=i&url=https%3A%2F%2Fburgosandbrein.com%2FFactors-and-How-to-Avoid-Them-3564442.html&psig=AOvVaw2B-rO60fph4Pk8A92Q3elk&ust=1709416737061000&source=images&cd=vfe&opi=89978449&ved=0CBMQjRxqFwoTCJjlid2H1IQDFQAAAAAdAAAAABAE)

## Overview of the Analysis

This analysis aims to create a supervised machine learning model that can predict the status of a potential loan as *healthy* or *high-risk*. The following features were used as input variables to develop the model:

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
* [x] The predictions were compared to the testing output data utilizing a `confusion_matrix` and a `classification_report`.

## Results

### Logistic Regression Model Performance:
  * **Model Accuracy Score:** _99%_
  * **Healthy Loan Predictions**
    * **Precision:** _100%_
    * **Recall:** _100%_
  * **High-Rish Loan Predictions**
    * **Precision:** _87%_
    * **Recall:** _98%_

## Summary

Overall, the machine learning model performed well with an accuracy score of 99%. For this analysis, it is more important for the model to successfully predict high-risk loans to avoid potential borrowers defaulting on their loans. While the model does a great job of identifying healthy loans, it performed slightly worse at predicting high-risk loans. The model had a very high recall ability for high-risk loans, meaning it had very few false negative predictions (loans that were actually high-risk being identified as healthy). This supports the purpose of the model in identifying potential risks. On the other hand, precision was lower at 87%, meaning there was a higher number of false positive predictions (loans that were actually healthy being identified as high-risk). While this isn't a great finding, it is preferable for the model to be overcautious with its predictions. **Therefore, I would recommend that the bank utilize this model as it does a satisfactory job of identifying high-risk borrowers.** _There is still room to improve the model in terms of avoiding incorrectly identifying healthy borrowers as high-risk. Perhaps different machine learning models could be tested as well to see if there is a better option._
