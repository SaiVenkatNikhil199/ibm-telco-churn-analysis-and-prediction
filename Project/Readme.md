Here’s a polished README you can directly use for your GitHub repository.

# IBM Telco Customer Churn Analysis & Prediction

## Overview

This project focuses on analyzing and predicting customer churn using the IBM Telco Customer Churn dataset. The project follows a complete end-to-end Machine Learning workflow involving data preprocessing, exploratory data analysis (EDA), feature engineering, imbalance handling, model training, evaluation, and explainability.

The primary objective of this project is to identify the major factors influencing customer churn and build a machine learning model capable of predicting customers who are likely to leave the telecom service.

---

# Problem Statement

Customer churn is one of the major business challenges faced by telecom companies. Losing existing customers leads to revenue loss and increased customer acquisition costs.

This project aims to:

* Analyze customer behavior patterns
* Identify churn-driving factors
* Build predictive models for churn detection
* Generate business insights that can help improve customer retention strategies

---

# Dataset

Dataset Used:

* IBM Telco Customer Churn Dataset

The dataset contains customer demographic information, account details, subscribed services, billing information, and churn status.

Target Variable:

* `Churn` (Yes / No)

---

# Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* imbalanced-learn (SMOTE)

---

# Project Workflow

## 1. Data Cleaning & Preprocessing

* Handled missing values
* Converted data types
* Encoded categorical variables using one-hot encoding
* Scaled numerical features using `StandardScaler`

---

# 2. Exploratory Data Analysis (EDA)

Performed detailed exploratory analysis to understand customer churn behavior.

Key analyses included:

* Contract type impact on churn
* Tenure vs churn analysis
* Payment method analysis
* Monthly charges analysis
* Internet service impact
* Senior citizen effect
* Service-related churn behavior

---

# 3. Feature Engineering

* One-hot encoding using `pd.get_dummies()`
* Numerical feature scaling using `StandardScaler`
* Pipeline-based preprocessing and model training

---

# 4. Machine Learning Models

Implemented Logistic Regression-based churn prediction models:

### Baseline Logistic Regression

Initial model trained on original imbalanced dataset.

### Balanced Logistic Regression

Used `class_weight='balanced'` to improve minority class learning.

### SMOTE + Logistic Regression

Applied SMOTE (Synthetic Minority Oversampling Technique) to address class imbalance and improve churn recall.

---

# 5. Model Evaluation

Models were evaluated using:

* Confusion Matrix
* Precision
* Recall
* F1-score
* Accuracy
* Comparative metric visualization

Special focus was placed on Recall and F1-score since identifying churn customers is more important than maximizing raw accuracy in churn prediction problems.

---

# 6. Explainability & Insights

Feature importance analysis revealed several strong churn indicators:

* Month-to-month contracts
* Electronic check payment method
* Fiber optic internet service
* High monthly charges
* Low tenure
* Lack of TechSupport and OnlineSecurity services

The explainability analysis closely aligned with the findings obtained during EDA.

---

# Key Business Insights

* Customers with month-to-month contracts show significantly higher churn rates.
* Customers with low tenure are more likely to churn.
* Electronic check users exhibit higher churn tendencies.
* High monthly charges contribute to increased churn probability.
* Customers without additional support/security services churn more frequently.
* Long-term contract customers demonstrate stronger customer retention.

---

# Results

Applying imbalance handling techniques such as:

* `class_weight='balanced'`
* SMOTE oversampling

significantly improved the model’s ability to identify churn customers, especially improving Recall and F1-score.

---

# Future Improvements

Potential future enhancements:

* Random Forest / XGBoost comparison
* Hyperparameter tuning
* Cross-validation
* SHAP explainability
* Streamlit deployment
* Real-time churn prediction dashboard

---

# Conclusion

This project demonstrates a complete end-to-end machine learning workflow for customer churn prediction and business analysis. The project combines data analysis, machine learning, explainability, and business interpretation to provide actionable insights for telecom customer retention strategies.

---

# Repository Structure

```bash
├── Project/
|    --  ibm_telco_churn_analysis.ipynb  
├── telco_churn.csv
├── README.md

```

---

# Author

Sai Venkat Nikhil
