# Titanic Survival Prediction - Feature Engineering Project

## Project Overview

This project focuses on applying a complete feature engineering workflow to the Titanic dataset.

The objective is to predict passenger survival using data preprocessing, feature engineering, and machine learning pipelines.

This project follows a structured industry-style workflow:

EDA
→ Feature Engineering
→ ML Pipeline
→ Model Evaluation

---

## Problem Statement

Predict whether a passenger survived the Titanic disaster based on:

- Passenger Class
- Gender
- Age
- Fare
- Family Information
- Embarkation Port

Target Variable:

- Survived
    - 0 = Did Not Survive
    - 1 = Survived

---

## Project Structure

titanic/
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
- Outlier analysis
- Correlation analysis
- Target variable analysis
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

- FamilySize
- IsAlone
- Title

---

### 03_ml_pipeline.ipynb

Production-style preprocessing workflow

Includes:

- Train-test split
- ColumnTransformer
- Pipeline
- Logistic Regression
- Model evaluation
- Feature engineering comparison

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn

---

## Key Learnings

- Handling missing values
- Feature creation
- Encoding categorical variables
- Numerical transformations
- Pipeline development
- Model evaluation
- End-to-end machine learning workflow

---

## Results

Multiple feature engineering experiments were conducted to evaluate the impact of engineered features on model performance.

The final workflow demonstrates a reusable and production-ready preprocessing pipeline.

---

## Author

Aditya Zadke

Feature Engineering Learning Track