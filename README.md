#README

# 🛡 AI-Powered Fraud Detection in Auto Insurance

This project is designed to detect fraudulent claims in auto insurance using historical data and machine learning. The solution leverages data preprocessing, classification models, and data visualization dashboards to help insurers reduce fraud, automate claim processing, and gain actionable business insights.

---

## 📌 Problem Statement

Insurance fraud leads to substantial financial losses. The goal is to build a predictive model that flags potentially fraudulent claims (Fraud_Ind = 'Y') based on features such as customer profile, policy details, vehicle information, and accident circumstances.

---

## 🚀 Project Objectives

- Detect fraudulent auto insurance claims
- Identify key features that drive fraud
- Create an interactive Power BI dashboard for visual exploration
- Generate business insights for use cases beyond fraud detection

---

## 📂 Dataset Overview

The dataset includes the following:

- *Customer Data*: Age, gender, education, occupation, hobbies
- *Policy Data*: Premium, deductible, liability limits, dates
- *Accident Data*: Date, hour, type, severity, location, police report
- *Vehicle Data*: Make, model, year, color, cost, mileage
- *Claim Data*: Total claimed, breakdown by type, claim date
- *Target Variable*: Fraud_Ind (Y/N)

---

## 🛠 Approach
The project aims to identify fraudulent auto insurance claims using a supervised classification approach. 
It performs preprocessing and compares multiple machine learning models to evaluate which performs best 
in terms of detecting fraud accurately.

📌 Includes:
- Dataset loading and inspection
- Data cleaning and preprocessing
- Label encoding and scaling
- Multiple classification models:
  • Logistic Regression
  • Random Forest
  • XGBoost
  • LightGBM
  • SVM
  • KNN
  • Naive Bayes
  • Decision Trees
  • LDA & QDA
- Model evaluation using:
  • Accuracy
  • Precision
  • Recall
  • F1 Score
  • Confusion Matrix
  • ROC AUC Score

### 1. Data Preprocessing
- Handled missing values (Police_Report, authorities_contacted)
- Converted date columns and calculated Claim_Delay
- Encoded categorical variables
- Created Fraud_Flag as binary target (1 = Fraud, 0 = Genuine)

### 2. Model Building
- Used *Random Forest Classifier* as baseline
- (Optional: Tested XGBoost, Logistic Regression)
- Evaluated with accuracy, precision, recall, and feature importance

### 3. Visualization
- Built interactive dashboards using:
  - *Power BI* (state-wise fraud, claim timing, vehicle risk)
  - *Streamlit* (model insights, fraud breakdown)

---

## 🧠 Why These Algorithms?

- *Random Forest*:
  - Excellent for mixed-type data
  - Interpretable (feature importance)
  - Less prone to overfitting
- *Classification models* (not regression) are suited since the target (Fraud_Ind) is binary

---

## 🏆 Results

- *Accuracy*: ~88–92%
- *Top Predictors*:
  - Accident_Severity
  - Policy_Expiry_Date
  - Insured_Zip
  - DL_Expiry_Date
- Dashboard insights revealed fraud patterns by location, vehicle type, time, and more.

---

## 💼 Business Use Cases

✅ *Fraud Detection*  
🧠 Flag risky claims for manual review

✅ *Faster Approvals*  
🧠 Auto-approve low-risk, low-value claims

✅ *Customer Retention*  
🧠 Use Customer_Life_Value and renewal dates to target churn

✅ *Safe Driver Scoring*  
🧠 Use behavior data to offer rewards or adjust pricing

✅ *Geographical Risk Mapping*  
🧠 Identify high-risk cities and ZIP codes for fraud or heavy claims

✅ *Vehicle Risk Analysis*  
🧠 Customize premiums based on make/model accident trends


---

## 📊 Tools Used

- Python (Pandas, scikit-learn, matplotlib, Streamlit)
- Google Colab Notebook
- CSV data files
