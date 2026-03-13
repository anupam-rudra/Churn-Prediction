## Customer Churn Prediction

# Project Overview

Customer churn is a critical problem for subscription-based businesses. Retaining an existing customer is often significantly cheaper than acquiring a new one.

This project builds machine learning models to predict whether a customer will churn based on demographic information, service usage, and account details.

The objective is to help companies identify high-risk customers and take proactive retention measures.


# Dataset

This project uses the Telco Customer Churn Dataset 

Features include:

Customer demographics

Account information

Service subscriptions

Monthly charges and tenure

Target variable:

Churn (Yes / No)

## Project Workflow
# Data Preprocessing
# Exploratory Data Analysis (EDA)
# Machine Learning Models(Churn_Prediction.ipynb)
# Model Evaluation
# Feature Importance


# Details about dataset 
The dataset named Telco Customer-Churn-csv is used.
Each row represents a customer, each column contains the customer's attributes. 
This dataset contains 21 columns (variables) and 7043 rows (customers) 
with information such as customerID, gender, Phone Service, and Internet Service. 
Table 1 shows the data types of the variables with 17 categorical and 4 numerical data.
Analysis of data columns to identify independent and dependent variables:

X is the independent variables - the variables we are using to make predictions

customerID - unique value identifying customer
gender - whether the customer is a male or a female
SeniorCitizen - whether the customer is a senior citizen or not (1, 0)
Partner - whether the customer has a partner or not (Yes, No)
Dependents - whether the customer has dependents or not (Yes, No). A dependent is a person who relies on another as a primary source of income,
tenure - number of months the customer has stayed with the company
PhoneService - whether the customer has a phone service or not (Yes, No)
MultipleLines - whether the customer has multiple lines or not (Yes, No, No phone service)
InternetService - customer’s internet service provider (DSL, Fiber optic, No)
OnlineSecurity - whether the customer has online security or not (Yes, No, No internet service)
OnlineBackup - whether the customer has online backup or not (Yes, No, No internet service)
DeviceProtection - whether the customer has device protection or not (Yes, No, No internet service)
TechSupport - whether the customer has tech support or not (Yes, No, No internet service)
StreamingTV - whether the customer has streaming TV or not (Yes, No, No internet service)

StreamingMovies - whether the customer has streaming movies or not (Yes, No, No internet service)
Contract - type of contract according to duration (Month-to-month, One year, Two year)
PaperlessBilling - bills issued in paperless form (Yes, No)
PaymentMethod - payment method used by customer (Electronic check, Mailed check, Credit card (automatic), Bank transfer (automatic))
MonthlyCharges - amount of charge for service on monthly bases
TotalCharges - cumulative charges for service during subscription (tenure) period
y is dependent variable - variable we are trying to predict or estimate

Churn – output value, predict variable
