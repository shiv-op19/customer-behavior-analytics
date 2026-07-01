# Project Retain – SaaS Customer Churn Prediction

## Overview

Customer churn is one of the biggest challenges faced by Software-as-a-Service (SaaS) companies. Acquiring a new customer is significantly more expensive than retaining an existing one. This project aims to analyze customer behavior, identify the factors contributing to churn, and build a machine learning model capable of predicting customers who are likely to leave the platform.

The project combines Exploratory Data Analysis (EDA), Machine Learning, and business insights to support proactive customer retention strategies.

---

## Problem Statement

The objective of this project is to:

* Analyze customer behavior using historical SaaS customer data.
* Identify important factors associated with customer churn.
* Build a machine learning model to predict churn.
* Generate churn risk scores for customers.
* Provide actionable business recommendations to improve customer retention.

---

## Dataset

The dataset contains customer information including:

* Customer_ID
* Name
* Email
* Account_Age_Days
* Login_Frequency
* Daily_Usage_Mins
* Last_Support_Ticket
* Churn (Target Variable)

**Target Variable**

* **Churn**

  * 0 → Customer Retained
  * 1 → Customer Churned

---

## Project Workflow

### 1. Data Preprocessing

* Removed irrelevant identifier columns (Customer_ID, Name, Email)
* Checked for missing values
* Cleaned the dataset
* Prepared features for model training

---

### 2. Exploratory Data Analysis (EDA)

Performed detailed analysis to understand customer behavior through visualizations and statistical observations.

Analysis included:

* Churn distribution
* Account age analysis
* Login frequency distribution
* Daily usage patterns
* Relationship between login frequency and daily usage
* Support ticket text exploration

Each visualization was accompanied by business insights.

---

### 3. Feature Engineering

* Numerical feature preprocessing
* TF-IDF Vectorization of support ticket text
* Feature combination for machine learning models

---

### 4. Machine Learning

Built a customer churn prediction model using supervised learning.

Workflow:

* Train/Test Split
* Model Training
* Model Evaluation
* Prediction Generation

Evaluation Metrics:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC Score
* Confusion Matrix

---

### 5. Churn Risk Scoring

Generated churn probabilities for every customer using the trained model.

Additional outputs include:

* Risk Score (0–1)
* Customer Risk Ranking
* High-Risk Customer Identification

These scores help businesses prioritize customer retention efforts.

---

## Business Insights

The analysis revealed several behavioral indicators associated with customer churn, including:

* Lower platform engagement
* Reduced login frequency
* Lower daily product usage
* Patterns observed from customer support interactions

These insights can help customer success teams proactively engage at-risk customers before they churn.

---

## Business Recommendations

Based on the analysis, the following strategies are recommended:

* Target high-risk customers with personalized retention campaigns.
* Improve customer onboarding to increase early engagement.
* Monitor declining login frequency as an early warning signal.
* Analyze support tickets to identify recurring customer pain points.
* Develop proactive customer success programs based on churn risk scores.

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Scikit-learn
* TF-IDF Vectorization
* Jupyter Notebook

---

## Project Deliverables

* Exploratory Data Analysis (EDA)
* Machine Learning Model
* Model Evaluation
* Customer Churn Predictions
* Churn Risk Score Generation
* CSV Output File
* Business Insights and Recommendations

---



## Future Improvements

* Hyperparameter optimization
* Model deployment using Flask or FastAPI
* Interactive dashboard using Streamlit
* Real-time churn prediction API
* Automated customer retention recommendation system

---
## Outputs

The project generates the following output files:

### 1. Churn Prediction Report
Contains predictions for all customers, including:
- Customer Identifier
- Predicted Churn Status
- Churn Probability (Risk Score)

This report helps businesses monitor the churn likelihood of their entire customer base.

### 2. High-Risk Customers Report
A filtered dataset containing customers with a high probability of churn.

This report enables customer success teams to:
- Prioritize retention campaigns
- Contact high-risk customers proactively
- Reduce potential customer loss

---

## Conclusion

This project demonstrates an end-to-end machine learning workflow for customer churn prediction in a SaaS environment. By combining data preprocessing, exploratory data analysis, predictive modeling, and business intelligence, the solution enables organizations to identify high-risk customers and take proactive actions to improve customer retention and long-term business growth.
