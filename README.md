# Machine Learning Project: Health Insurance Cross Sell Prediction 🏥

Hello everyone, thank you for being here! 😊

## Problem Statement and Business Goal

Our client is an Insurance company that has provided Health Insurance to its customers. They need our help in finding out whether the policyholders (customers) from past year will also be interested in Vehicle Insurance provided by the company.

Therefore, the aim of this project is to build a model to predict whether a customer would be interested in Vehicle Insurance. This is extremely helpful for the company because it can then accordingly plan its communication strategy to reach out to those customers and optimise its business model and revenue.

## The Dataset

The `train.csv` file contains the following variables:

* `Gender`: Gender of the customer;
* `Age`: Age of the customer;
* `Driving_License`:
  * 0 : Customer doesn't have DL;
  * 1 : Customer already has DL.
* `Region_Code`: Unique code for the region of the customer;
* `Previously_Insured`:
  * 0 : Customer doesn't have Vehicle Insurance;
  * 1 : Customer already has Vehicle Insurance.
* `Vehicle_Age`: Age of the Vehicle;
* `Vehicle_Damage`:
  * 0 : Customer didn't get his/her vehicle damaged in the past;
  * 1 : Customer got his/her vehicle damaged in the past.
* `Annual_Premium`: The amount customer needs to pay as premium in the year.
* `Policy_Sales_Channel`: Anonymized Code for the channel of outreaching to the customer ie. Different Agents, Over Mail, Over Phone, In Person, etc.;
* `Vintage`: Number of Days, Customer has been associated with the company;
* `Response`:
  * 0 : Customer isn't interested in Vehicle Insurance provided by the company;
  * 1 : Customer is interested in Vehicle Insurance provided by the company.

On the other hand, the `test.csv` file contains the same variables as `train.csv` but `Response`, which represents the target variable of our problem, namely the variable to predict.

## Brief Summary

The first part of the project is dedicated to analyzing the relationships between the features and the target variable, and properly preparing the dataset for the second part of the project, which consists of building different models and choosing the best one, based on the value of precision and recall. In particular, we address the problem of class imbalance using different approaches, that are: 

* to give different weights to the majority and minority classes;
* to delete instances from the majority class (undersampling);
* to duplicate examples from the minority class (oversampling);
* `SMOTENC`, i.e. an extension of the Synthetic Minority Oversampling Technique (SMOTE) that can be used also in the presence of categorical data among the features.


