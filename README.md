# Lending Club Loan Default Prediction

## 1. Business Understanding
This project aims to build a machine learning model that predicts the probability of loan default for Lending Club customers. 
Accurate default prediction enables financial institutions to reduce credit risk, optimize approval decisions, and improve portfolio profitability.

## 2. Data Understanding
The dataset contains historical loan applications with borrower demographics, loan attributes, and credit history information.
Target variable: loan_status (converted to binary: Default vs Fully Paid).

Key feature groups:
- Borrower Profile: income, employment length, home ownership
- Loan Details: loan amount, interest rate, term
- Credit History: debt-to-income, delinquencies, revolving utilization, open accounts

Exploratory analysis identified strong relationships between default risk and interest rate, DTI, credit utilization, and income.

## 3. Data Preparation
- Removed leakage and irrelevant columns
- Imputed missing values using median/mode strategy
- Encoded categorical features with one-hot encoding
- Engineered new features such as credit utilization ratio and income-to-loan ratio
- Addressed class imbalance using resampling techniques
- Final dataset standardized and split into training and test sets

## 4. Modeling
Models trained:
- Logistic Regression
- Random Forest
- Gradient Boosting
- XGBoost / LightGBM

Hyperparameter tuning performed using cross-validation.
Final model selected based on ROC-AUC and recall for default class.

## 5. Evaluation
Evaluation metrics:
- Accuracy
- Precision, Recall, F1-score
- ROC-AUC
- Confusion Matrix

Model achieved strong discrimination between default and non-default customers.
Feature importance analysis highlighted interest rate, DTI, credit utilization, income, and loan amount as top drivers.

## 6. Business Impact & Deployment
The model can be integrated into loan approval pipelines for:
- Automated risk scoring
- Risk-based pricing
- Portfolio risk monitoring

Expected benefits:
- Reduced default losses
- Faster decision cycles
- Improved capital efficiency

## 7. Conclusion
This project demonstrates a full CRISP-DM lifecycle and delivers a production-ready credit risk prediction system.

Author: Swaroop Narayan
