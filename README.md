# Telecom Customer Churn Analysis
Telecom Customer Churn Analysis

## 📌 Overview
This project analyzes customer churn patterns for a telecom company. The dashboard identifies key churn drivers such as contract type, tenure, and service usage.

## 🎯 Objectives
- Measure overall churn rate and retention rate
- Identify customer segments most likely to churn
- Support data-driven customer retention strategies

## 📂 Dataset
- Source: Telco Customer Churn Dataset - Kaggle
- Description: 7,043 customer records including demographics, services subscribed, tenure, and churn status.

## 🛠 Tools & Technologies
- SQL (data filtering, grouping, segmentation)
- Power BI (churn dashboard)
- DAX (Churn Rate, Retention Rate, Avg Tenure of Churned Customers)

## 📊 Key DAX Measures
Churn Rate = DIVIDE(COUNTROWS(FILTER(Customers, Customers[Churn] = "Yes")), COUNTROWS(Customers))
Retention Rate = 1 - [Churn Rate]
Avg Tenure Churned = AVERAGEX(FILTER(Customers, Customers[Churn] = "Yes"), Customers[Tenure])

