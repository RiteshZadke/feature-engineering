# Loan Prediction - Feature Engineering Project

## Project Overview

This project focuses on building a complete feature engineering and machine learning workflow for loan approval prediction.

The objective is to identify factors influencing loan approval decisions and build a reusable preprocessing pipeline.

Workflow:

EDA
→ Feature Engineering
→ ML Pipeline
→ Model Evaluation

---

## Problem Statement

Predict whether a loan application will be approved based on applicant information.

Target Variable:

- Loan_Status

Classes:

- Y = Approved
- N = Rejected

---

## Business Objective

Financial institutions must evaluate loan applications efficiently while minimizing credit risk.

This project aims to:

- Understand borrower characteristics
- Identify important approval factors
- Engineer meaningful features
- Build a scalable preprocessing pipeline

---

## Project Structure

loan-prediction/
│
├── 01_eda.ipynb
├── 02_feature_engineering.ipynb
├── 03_ml_pipeline.ipynb
└── dataset/

---

## Notebook Description

### 01_eda.ipynb

Exploratory Data Analysis

Includes:

- Dataset overview
- Missing value analysis
- Numerical analysis
- Categorical analysis
- Target variable analysis
- Correlation analysis
- Feature engineering opportunities
- Preprocessing decisions

---

### 02_feature_engineering.ipynb

Manual Feature Engineering

Includes:

- Missing value handling
- Feature creation
- Manual encoding
- Transformations
- Outlier treatment
- Scaling
- Validation

Engineered Features:

- TotalIncome
- LoanIncomeRatio
- IncomePerPerson
- Log-transformed income features

---

### 03_ml_pipeline.ipynb

Production-style ML workflow

Includes:

- Train-test split
- SimpleImputer
- OneHotEncoder
- StandardScaler
- ColumnTransformer
- Pipeline
- Logistic Regression
- Model evaluation

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

---

## Feature Engineering Highlights

### Income Features

Created:

- TotalIncome
- LoanIncomeRatio

These features provide a better representation of repayment capability than raw income variables.

---

### Data Transformations

Applied:

- Log transformation
- Missing value imputation
- Categorical encoding
- Numerical scaling

---

## Key Learnings

- Credit risk preprocessing
- Business-driven feature engineering
- Handling missing values
- Categorical encoding
- Pipeline construction
- Classification model evaluation

---

## Results

Baseline and feature-engineered models were compared to measure the impact of engineered features on loan approval prediction.

The final solution demonstrates a complete end-to-end preprocessing and machine learning workflow.

---

## Author

Ritesh Zadke

Feature Engineering Learning Track