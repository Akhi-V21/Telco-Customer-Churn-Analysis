# Customer Churn Analysis and Prediction
### Internship Project - SaiKet Systems Developed by: Akhila Vaidya

## 1. Problem Statement
The goal of this project is to analyze the Telco Customer Churn dataset to identify why customers are leaving and to build a predictive model that can flag "at-risk" customers. By understanding these patterns, the business can take proactive steps to improve customer retention.

## 2. Business Problem Overview
In the telecommunications industry, the cost of acquiring a new customer is significantly higher than retaining an existing one. High churn rates directly impact profitability. This project provides data-driven insights to help the business understand customer behavior and reduce turnover.

## 3. Understanding and Defining Churn
Churn is defined as the loss of clients or customers. In this dataset, churn is a binary variable:

Yes: The customer left the company within the last month.

No: The customer remained with the company.

## 4. High-Value Churn
A key focus of this analysis is identifying "High-Value" customers—those with high Monthly Charges and long Tenure—who are at risk of churning. Losing these customers has the most significant financial impact on the company.

## 5. Understanding the Business Objective and the Data
The primary objectives are:

Identify key demographic and service-related factors leading to churn.

Clean and preprocess raw data for machine learning.

Build a model to predict the probability of a customer leaving.

Propose actionable retention strategies.

## 6. Understanding Customer Behaviour During Churn
Through Exploratory Data Analysis (EDA), we observed several patterns:

Contract Type: Customers on Month-to-month contracts churn at a much higher rate than those on one or two-year contracts.

Payment Method: Electronic check users show a higher tendency to churn.

Services: Customers without tech support or online security are more likely to leave.

## 7. Dataset and Data Dictionary
The project uses the Telco_Customer_Churn_Dataset.csv. Key features include:

CustomerID: Unique ID for each customer.

Tenure: Number of months the customer has stayed with the company.

MonthlyCharges: The amount charged to the customer monthly.

TotalCharges: The total amount charged to the customer.

Churn: Whether the customer churned or not (Target Variable).

## 8. Data Preparation
To prepare the data for modeling, the following steps were taken:

Handling Missing Values: Converted TotalCharges to numeric and filled null values.

Encoding: Converted categorical variables (like Gender and Contract) into numerical format using One-Hot Encoding and Label Encoding.

Feature Scaling: Ensured numerical features were on a similar scale for better model performance.

## 9. Modelling
I developed a Logistic Regression model to predict churn.

Algorithm: Logistic Regression (chosen for its efficiency in binary classification).

Training: The data was split into 80% training and 20% testing sets.

Performance: The model achieved a baseline accuracy score (e.g., ~80%), allowing the business to identify potential churners effectively.

## 10. Conclusion and Strategies
Based on the model and analysis, the following strategies are proposed:

Encourage Month-to-month customers to switch to one-year contracts through discounts.

Target "High-Value" customers with loyalty rewards.

Improve Tech Support and Online Security offerings to increase customer stickiness.



