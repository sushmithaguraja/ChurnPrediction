# ChurnPrediction

# 🎬 Churn Prediction Challenge

This project is part of Coursera’s **Data Science Coding Challenge**, where the goal is to predict **customer churn** for a video streaming service using real-world subscription data.

---

## 📖 Project Overview

Subscription-based companies rely heavily on understanding which customers are likely to cancel their services (“churn”).  
In this project, I built a **machine learning model** that predicts the likelihood of a customer continuing their subscription for another month.

The project involves:
- Data cleaning and preprocessing
- Feature exploration and encoding
- Model training and evaluation
- Generating churn probability predictions for new users

---

## 📂 Dataset

Two datasets were provided:

| File | Description |
|------|--------------|
| `train.csv` | 243,787 customer records with churn labels (1 = churned, 0 = retained) |
| `test.csv` | 104,480 customer records without churn labels — used for prediction submission |

Each record represents one subscription and includes features like:
- **AccountAge** (months)
- **MonthlyCharges**, **TotalCharges**
- **SubscriptionType** (Basic, Standard, Premium)
- **ContentType**, **ViewingHoursPerWeek**
- **UserRating**, **SupportTicketsPerMonth**, etc.

---

## 🧠 Approach

1. **Data Preprocessing**
   - Handled missing values
   - Encoded categorical features with LabelEncoder / OneHotEncoder
   - Scaled numeric variables

2. **Modeling**
   - Tried multiple models (Logistic Regression, Random Forest, Gradient Boosting)
   - Evaluated performance using **ROC AUC**

3. **Evaluation**
   - Metric used: **Area Under the ROC Curve (**
