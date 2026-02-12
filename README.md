# Customer Churn Analysis and Prediction
### Internship Project - SaiKet Systems Developed by: Akhila Vaidya1.
## Problem Statement:
The goal of this project is to analyze the Telco Customer Churn dataset to identify why customers are leaving and to build a predictive model. The focus is on identifying patterns in customer behavior that lead to service termination.

## 2. Business Problem Overview:
In the telecom industry, retaining a customer is cheaper than acquiring a new one. This project addresses the business need to reduce "Churn" (loss of customers) by providing data-driven insights and a predictive tool for the retention team.

## 3. Understanding and Defining Churn
In this project, Churn is defined based on the service model:

1.Contract-Based Churn: Customers on one or two-year contracts who choose not to renew.

2.Month-to-Month Churn: Customers who pay monthly and can stop the service at any time.

This is the most volatile segment and requires the most attention.

## 4. High-Value Churn
Following the SaiKet Systems objective, this project prioritizes "High-Value" customers.
We define these as customers with high Monthly Charges and significant Tenure. Losing these customers represents a major revenue loss, so the model specifically looks for risks in this group.

## 5. Understanding the Business Objective and the Data:
The objective is to move from raw data to actionable strategy:

1.Clean the data to ensure accuracy.

2.Analyze which services (Internet, Tech Support, etc.) correlate with loyalty.

3.Predict future churn using Machine Learning.

## 6. Understanding Customer Behaviour During Churn
Based on the Exploratory Data Analysis (EDA) in my notebooks:

1.Fiber Optic users show a higher churn rate compared to DSL users.

2.Newer customers (low tenure) are at a higher risk of leaving than long-term customers.

3.Lack of Online Security/Tech Support is a leading indicator that a customer might churn.

## 7. Dataset and Data Dictionary
The dataset contains 7,043 rows and 21 columns.

You can download dataset [![Download CSV](https://img.shields.io/badge/Download-Dataset-blue(Telco_Customer_Churn_Dataset.csv)

Key features include:

1.Tenure: Number of months the customer stayed.

2.MonthlyCharges: The amount charged each month.

3.Contract: The contract term (Month-to-month, One year, Two year).

4.Churn: Whether the customer left or not (Target).

## 8. Data PreparationI performed the following steps to prepare the data:
Handling Nulls: Converted TotalCharges to numeric and handled missing values.

Encoding: Used get_dummies to convert categorical text (like "Yes/No") into numbers ($0$ and $1$) that the model can read.

Feature Selection: Dropped customerID as it has no predictive power.

## 9. ModellingI built a Logistic Regression model to classify customers:
Training: 80% of the data was used to teach the model.

Testing: 20% was used to verify accuracy.

Result: The model provides a clear "Churn Probability" for every customer.

## 10. Data-Driven Retention Strategies :
Based on my findings, I recommend:

Convert to Contracts: Offer small discounts to move Month-to-Month users to 1-year plans.

Tech Support Bundles: Provide free or discounted Tech Support to Fiber Optic users to increase "stickiness.

"Loyalty Programs: Target high-tenure, high-value customers with proactive rewards before they reach their "churn window."

