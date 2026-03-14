# 📊 Telco Customer Churn Prediction

## 📌 Project Overview
Customer churn is a major challenge for telecom companies because losing customers directly affects revenue. Predicting churn helps businesses identify customers who are likely to leave and take proactive actions to retain them.

This project analyzes the **Telco Customer Churn dataset** and builds multiple machine learning models to predict whether a customer will churn. The project includes data cleaning, exploratory data analysis (EDA), feature engineering, model training, hyperparameter tuning, and performance evaluation.

---

## 📂 Dataset

The dataset contains information about telecom customers including demographics, services subscribed, billing information, and whether the customer churned.

### Key Features

**Customer Information**
- `gender`
- `SeniorCitizen`
- `Partner`
- `Dependents`

**Service Information**
- `PhoneService`
- `InternetService`
- `OnlineSecurity`
- `StreamingTV`
- `TechSupport`

**Account Information**
- `tenure`
- `Contract`
- `PaperlessBilling`
- `PaymentMethod`

**Billing Information**
- `MonthlyCharges`
- `TotalCharges`

**Target Variable**
- `Churn` (Yes / No)

---

## 🧹 Data Preprocessing

The following preprocessing steps were performed:

- Converted `TotalCharges` to numeric values
- Handled missing values
- Removed rows with null values
- Converted `Churn` from Yes/No to binary (1/0)
- Created tenure groups for lifecycle analysis
- Applied One-Hot Encoding for categorical variables
- Scaled features using `StandardScaler`

---

## 📊 Exploratory Data Analysis (EDA)

Several visualizations were created to understand the data and customer behavior:

- Churn distribution plot
- Churn percentage pie chart
- Correlation heatmap
- Churn rate by contract type
- Tenure distribution histogram

These visualizations help identify patterns and relationships related to churn.

---

## 🤖 Machine Learning Models

Three machine learning models were implemented in this project.

### 1️⃣ Logistic Regression
Used as a baseline model to understand the relationship between features and churn.

Steps performed:
- Model training
- Confusion matrix
- ROC-AUC evaluation
- ROC curve visualization
- Optimal threshold selection using Youden Index

---

### 2️⃣ Random Forest Classifier

An ensemble tree-based model capable of capturing nonlinear relationships in the data.

Key steps:
- Hyperparameter tuning using `RandomizedSearchCV`
- Model evaluation using classification metrics
- ROC-AUC score analysis
- Feature importance extraction

---

### 3️⃣ XGBoost Classifier

A gradient boosting model known for strong predictive performance.

Key steps:
- Hyperparameter tuning using `RandomizedSearchCV`
- ROC-AUC evaluation
- Feature importance analysis
- Optimal cutoff threshold calculation

---

## 📈 Model Evaluation Metrics

Models were evaluated using the following metrics:

- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix
- ROC-AUC Score
- Gini Coefficient
- ROC Curve

The **optimal probability threshold** was also determined using:

- Youden Index
- Minimum distance to top-left corner of ROC curve

---

## 🔍 Feature Importance

Feature importance analysis was conducted for tree-based models to identify factors that influence customer churn.

Important factors typically include:

- Contract type
- Tenure
- Monthly charges
- Internet services
- Payment method

These insights help telecom companies design effective customer retention strategies.


##  Key Insights

- Customers with **month-to-month contracts** are more likely to churn.
- Customers with **short tenure** have higher churn probability.
- Higher **monthly charges** are associated with increased churn risk.
- Service combinations and contract types influence customer retention.

