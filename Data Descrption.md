## Customer Churn Prediction

# Project Overview

Customer churn is a critical problem for subscription-based businesses. Retaining an existing customer is often significantly cheaper than acquiring a new one.

This project builds machine learning models to predict whether a customer will churn based on demographic information, service usage, and account details.

The objective is to help companies identify high-risk customers and take proactive retention measures.


# 📑 Data Description



The dataset used in this project is **Telco-Customer-Churn.csv**.  
Each row in the dataset represents a **single customer**, and each column represents the **customer's attributes or characteristics**.

The dataset contains:

- **7043 rows (customers)**
- **21 columns (variables)**

These variables include customer demographics, services subscribed, billing details, and the customer's churn status.

Among the variables:

- **17 are categorical variables**
- **4 are numerical variables**

---

# 🔍 Variables and Features

## Independent Variables (X)

Independent variables are the features used to **predict customer churn**.

### Customer Information

- **customerID**  
  Unique identifier for each customer.

- **gender**  
  Whether the customer is **Male** or **Female**.

- **SeniorCitizen**  
  Indicates whether the customer is a senior citizen.  
  - 1 = Yes  
  - 0 = No

- **Partner**  
  Indicates whether the customer has a partner.  
  - Yes  
  - No

- **Dependents**  
  Indicates whether the customer has dependents.  
  - Yes  
  - No  

  A dependent is a person who relies on another individual as a primary source of income.

---

### Account Information

- **tenure**  
  Number of months the customer has stayed with the company.

- **Contract**  
  Type of contract the customer has with the company.  
  - Month-to-month  
  - One year  
  - Two year

- **PaperlessBilling**  
  Indicates whether billing is done electronically.  
  - Yes  
  - No

- **PaymentMethod**  
  Payment method used by the customer.  
  - Electronic check  
  - Mailed check  
  - Credit card (automatic)  
  - Bank transfer (automatic)

---

### Phone Services

- **PhoneService**  
  Indicates whether the customer has phone service.  
  - Yes  
  - No

- **MultipleLines**  
  Indicates whether the customer has multiple phone lines.  
  - Yes  
  - No  
  - No phone service

---

### Internet Services

- **InternetService**  
  Type of internet service used by the customer.  
  - DSL  
  - Fiber optic  
  - No

- **OnlineSecurity**  
  Whether the customer has online security.  
  - Yes  
  - No  
  - No internet service

- **OnlineBackup**  
  Whether the customer has online backup.  
  - Yes  
  - No  
  - No internet service

- **DeviceProtection**  
  Whether the customer has device protection.  
  - Yes  
  - No  
  - No internet service

- **TechSupport**  
  Whether the customer receives technical support.  
  - Yes  
  - No  
  - No internet service

- **StreamingTV**  
  Whether the customer subscribes to streaming TV services.  
  - Yes  
  - No  
  - No internet service

- **StreamingMovies**  
  Whether the customer subscribes to streaming movie services.  
  - Yes  
  - No  
  - No internet service

---

### Billing Information

- **MonthlyCharges**  
  The amount charged to the customer **each month** for the services.

- **TotalCharges**  
  The **total cumulative amount charged** to the customer during the entire subscription period (tenure).

---

# 🎯 Dependent Variable (y)

The dependent variable represents the **target variable** that the model tries to predict.

- **Churn**  
  Indicates whether the customer left the company.

  - Yes → Customer churned  
  - No → Customer retained

This variable is the **output variable** used for classification in the churn prediction models.

---

# 📊 Summary

| Category | Description |
|--------|-------------|
| Rows | 7043 customers |
| Columns | 21 variables |
| Numerical Features | 4 |
| Categorical Features | 17 |
| Target Variable | Churn |

The dataset provides detailed customer information that allows machine learning models to identify patterns associated with **customer retention and churn behavior**.
