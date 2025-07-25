# 🚗 Auto Insurance Fraud Detection Project

## 🛠 Overview

This project focuses on detecting fraudulent auto insurance claims using supervised machine learning models. It performs data cleaning, preprocessing, exploratory data analysis (EDA), model training, evaluation, and selection of the best model for predictions.

---

## 📂 Dataset Description

The project uses the following datasets:

- `Auto_Insurance_Fraud_Claims_File01.csv`: Main training dataset
- `Auto_Insurance_Fraud_Claims_File02.csv`: Additional training dataset
- `Auto_Insurance_Fraud_Claims_File03.csv`: Test dataset
- `Auto_Insurance_Fraud_Claims_Results_Submission.csv`: Submission format

---

## 📌 Project Workflow

### 1. Data Cleaning & Preprocessing

- ✅ Removed duplicates
- ✅ Handled missing values (mode for categorical, median for numerical)
- ✅ Removed outliers using Interquartile Range (IQR)
- ✅ Label encoding for categorical columns
- ✅ Dropped non-useful columns like `Claim_ID`, `Policy_Start_Date`, etc.

---

### 2. Exploratory Data Analysis (EDA)

- 📊 Pie chart for class distribution (`Fraud_Ind`)
- 📊 Bar chart for top 5 `Claim_Type` (if present)
- 📊 Histograms for top KPIs like:
  - `Age`
  - `Days_To_Claim`
  - `Claim_Amount`
  - `Number_of_Damages`
  - `Policy_Holder_Age`

---

### 3. Model Building & Evaluation

Multiple models were trained and evaluated:

- 🔍 **Logistic Regression**
- 🌲 **Random Forest**
- 🧠 **Naive Bayes**
- 🔗 **Voting Classifier** (soft voting with LR, RF, NB)

Evaluation metrics used:
- Accuracy
- Precision
- Recall
- F1 Score
- Confusion Matrix (with heatmap)
- ROC AUC Score (if needed)

📈 Based on the comparison, the best performing model is selected for final prediction.

---

### 4. Final Prediction and Submission

- The selected model is used to predict fraud (`Fraud_Ind`) on the test dataset.
- Predictions are mapped to `Y` (Fraud) and `N` (Not Fraud)
- Output is saved to `Final_Submission.csv`.

---

## ✅ Results

- **Best Accuracy:** ~89–92% with Voting Classifier
- **Top Features Identified:**
  - `Accident_Severity`
  - `Claim_Amount`
  - `Policy_Expiry_Date`
  - `Insured_Zip`
  - `DL_Expiry_Date`

---

## 📊 Visualizations

- Seaborn & Matplotlib plots for distribution
- Confusion matrix heatmaps
- KPI charts
- (Optional) Streamlit / Power BI dashboards

---

## 💼 Business Use Cases

- 🔍 **Fraud Detection:** Automatically flag suspicious claims for manual review
- 🚀 **Faster Approvals:** Auto-approve safe, low-value claims
- 🧠 **Churn Prevention:** Use lifetime value and renewal status
- 🗺️ **Risk Mapping:** Identify fraud-prone ZIP codes and vehicle types
- 🚗 **Vehicle Scoring:** Adjust premiums based on vehicle accident trends

---

## 🧰 Tools & Libraries Used

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Scikit-learn (classification models)
- Google Colab (for development and execution)
- LabelEncoder, RandomForest, LogisticRegression, NaiveBayes, VotingClassifier

---

## 📁 Output Files

- `Final_Submission.csv` — test predictions with `Fraud_Ind` in Y/N format
- Confusion matrix and model performance metrics
- EDA charts

---

## 🚀 How to Run

1. Load all CSV files into the same directory.
2. Run the Jupyter Notebook / Python script.
3. Review EDA outputs and model performance.
4. Download or review `Final_Submission.csv`.

---

## 🤝 Contributing

Feel free to contribute improvements, alternate model suggestions, or dashboard enhancements!

---

## 📧 Contact

If you have questions or feedback, feel free to reach out.

