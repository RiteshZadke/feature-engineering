# Ames Housing Price Prediction - Feature Engineering Project

## Overview

This project focuses on building a complete Feature Engineering and Machine Learning workflow using the Ames Housing Dataset.

The objective is to predict residential property sale prices based on housing characteristics, property features, and neighborhood information.

The project follows an industry-style workflow:

**EDA → Feature Engineering → ML Pipeline → Model Evaluation**

---

## Problem Statement

Predict the final sale price of residential homes using property-related features.

### Target Variable

* SalePrice

### Problem Type

* Supervised Learning
* Regression

---

## Business Objective

Accurate house price prediction helps:

* Home buyers estimate fair property values
* Sellers determine competitive listing prices
* Real estate agencies improve valuation accuracy
* Financial institutions assess mortgage-related risks

---

## Project Structure

```text
ames-housing/
│
├── README.md
├── 01_eda.ipynb
├── 02_feature_engineering.ipynb
├── 03_pipeline_workflow.ipynb
└── dataset/
```

---

## Workflow

### 1. Exploratory Data Analysis

Objectives:

* Dataset understanding
* Missing value analysis
* Numerical feature analysis
* Categorical feature analysis
* Outlier detection
* Correlation analysis
* Target variable analysis
* Feature engineering opportunities
* Preprocessing decisions

---

### 2. Feature Engineering

Objectives:

* Missing value handling
* Binary feature creation
* Domain-driven feature engineering
* Log transformation
* Ordinal encoding
* One-hot encoding
* Feature validation

### Engineered Features

* HasGarage
* HasPool
* HasFireplace
* HasBasement
* TotalSF
* HouseAge
* RemodelAge
* TotalBath
* TotalPorchSF

---

### 3. Machine Learning Pipeline

Objectives:

* Train-Test Split
* Automated preprocessing
* Ordinal Encoding
* One-Hot Encoding
* Power Transformation
* Feature Scaling
* ColumnTransformer
* Pipeline Development
* Regression Modeling
* Model Comparison

---

## Dataset Challenges

### Missing Values

Several features contain missing values that represent the absence of a property characteristic rather than missing information.

Examples:

* PoolQC
* FireplaceQu
* Alley
* GarageType
* Fence

These features require domain-specific handling.

---

### Ordinal Features

Many housing quality variables contain natural ordering.

Examples:

```text
Ex > Gd > TA > Fa > Po
```

Examples:

* ExterQual
* KitchenQual
* FireplaceQu
* GarageCond
* GarageQual

These features were handled using ordinal encoding.

---

## Feature Engineering Highlights

### Total Living Space

Created:

```python
TotalSF = TotalBsmtSF + 1stFlrSF + 2ndFlrSF
```

---

### Property Age

Created:

```python
HouseAge = YrSold - YearBuilt
```

---

### Remodel Age

Created:

```python
RemodelAge = YrSold - YearRemodAdd
```

---

### Binary Indicators

Created:

* HasGarage
* HasPool
* HasFireplace
* HasBasement

These features capture the presence or absence of important housing characteristics.

---

## Machine Learning Pipeline

The preprocessing workflow uses:

* SimpleImputer
* OrdinalEncoder
* OneHotEncoder
* PowerTransformer
* StandardScaler
* ColumnTransformer
* Pipeline

Benefits:

* Automated preprocessing
* Reduced data leakage
* Train-test consistency
* Reproducible workflow

---

## Models Used

### Baseline Model

Uses original dataset features.

### Feature Engineered Model

Uses engineered features created during preprocessing.

Both models are compared to evaluate the impact of feature engineering.

---

## Evaluation Metrics

Regression models were evaluated using:

* Mean Absolute Error (MAE)
* Root Mean Squared Error (RMSE)
* R² Score

---

## Key Learnings

* Advanced Missing Value Handling
* Ordinal Encoding
* One-Hot Encoding
* Feature Engineering
* Power Transformation
* Pipeline Development
* Regression Modeling
* Model Evaluation

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

A baseline model and a feature-engineered model were developed and compared.

The project demonstrates how domain-driven feature engineering and automated preprocessing pipelines can improve regression model performance while maintaining a clean and reproducible workflow.

---

## Author

Ritesh Zadke

Aspiring Data Scientist | Feature Engineering Portfolio
