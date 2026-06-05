# Adult Income Prediction - Feature Engineering Project

## Project Overview

This project focuses on applying feature engineering, preprocessing pipelines, and machine learning techniques to the Adult Income Census Dataset.

The objective is to predict whether an individual's annual income exceeds $50,000 based on demographic, educational, and employment-related information.

The project follows a structured workflow:

EDA → Feature Engineering → ML Pipeline → Model Evaluation

---

## Problem Statement

Predict whether an individual's annual income is:

* <=50K
* > 50K

based on personal and employment characteristics.

Target Variable:

* income

Problem Type:

* Binary Classification

---

## Business Objective

Organizations and government agencies often need to understand income patterns across populations.

This project aims to:

* Analyze demographic and employment factors affecting income levels.
* Engineer meaningful features from raw census data.
* Build reusable preprocessing pipelines.
* Evaluate the impact of feature engineering on model performance.

---

## Project Structure

```text
adult-income/
│
├── README.md
├── 01_eda.ipynb
├── 02_feature_engineering.ipynb
├── 03_ml_pipeline.ipynb
└── dataset/
```

---

## Notebook Description

### 01_eda.ipynb

Exploratory Data Analysis

Includes:

* Dataset overview
* Missing value analysis
* Numerical feature analysis
* Categorical feature analysis
* Target variable analysis
* Correlation analysis
* Feature engineering opportunities
* Preprocessing decisions

---

### 02_feature_engineering.ipynb

Manual Feature Engineering

Includes:

* Missing value handling
* Feature creation
* Categorical encoding
* Data transformations
* Feature validation
* Scaling techniques

Engineered Features:

* AgeGroup
* WorkHoursCategory
* MaritalGroup
* EducationGroup
* OccupationGroup
* RegionGroup

---

### 03_ml_pipeline.ipynb

Production-style preprocessing and modeling workflow

Includes:

* Train-test split
* Custom feature transformer
* SimpleImputer
* OneHotEncoder
* StandardScaler
* ColumnTransformer
* Pipeline
* Logistic Regression
* Baseline vs Feature Engineered comparison

---

## Dataset Features

### Numerical Features

* age
* education-num
* capital-gain
* capital-loss
* hours-per-week

### Categorical Features

* workclass
* education
* marital-status
* occupation
* relationship
* race
* sex
* native-country

### Target Feature

* income

---

## Feature Engineering Highlights

### Age Grouping

Created age categories to capture different career stages and earning patterns.

### Work Hour Categories

Grouped working hours into meaningful categories to represent work intensity.

### Education Grouping

Combined education levels into broader educational attainment categories.

### Marital Status Simplification

Reduced category complexity while preserving meaningful information.

### Occupation Grouping

Grouped similar occupations into broader employment categories.

### Region Grouping

Grouped countries into geographical regions to reduce cardinality.

---

## Machine Learning Pipeline

The preprocessing workflow is fully automated using:

* SimpleImputer
* StandardScaler
* OneHotEncoder
* ColumnTransformer
* Pipeline

Benefits:

* Reproducible workflow
* Train-test consistency
* Reduced data leakage risk
* Production-ready preprocessing

---

## Model Evaluation

The project compares:

### Baseline Model

Uses original dataset features.

### Feature Engineered Model

Uses engineered features created during preprocessing.

Performance comparison helps determine whether engineered features improve predictive power.

---

## Key Learnings

* Missing value handling
* Feature engineering
* High-cardinality categorical preprocessing
* Encoding strategies
* Pipeline development
* Automated preprocessing
* Classification model evaluation
* Feature impact analysis

---

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn

---

## Results

Baseline and feature-engineered models were compared to evaluate the effectiveness of newly created features.

The final workflow demonstrates a complete end-to-end machine learning pipeline with reusable preprocessing and feature engineering components.

---

## Author

Ritesh Zadke

Aspiring Data Scientist | Feature Engineering Portfolio
