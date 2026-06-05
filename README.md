# Credit Risk Prediction Using Machine Learning

## Project Overview

This project develops a machine learning model to predict loan default risk using historical credit application data. The objective is to identify borrowers who are likely to default on their loans, enabling financial institutions to make more informed lending decisions and reduce financial risk.

The project follows a complete machine learning workflow, including exploratory data analysis (EDA), data preprocessing, feature engineering, model training, hyperparameter tuning, and performance evaluation.

---

## Dataset

The dataset used in this project is the Credit Risk Dataset, publicly available on Kaggle.

**Source:** https://www.kaggle.com/datasets/laotse/credit-risk-dataset

### Dataset Information

- Number of Records: 32,581
- Number of Features: 12
- Target Variable: `loan_status`
  - 0 = Non-default
  - 1 = Default

### Features Include

- Person Age
- Person Income
- Home Ownership Status
- Employment Length
- Loan Intent
- Loan Grade
- Loan Amount
- Interest Rate
- Loan Percentage Income
- Historical Default Information
- Credit History Length

---

## Project Workflow

### 1. Data Understanding

- Loaded and inspected the dataset
- Reviewed data types and feature distributions
- Examined summary statistics

### 2. Data Cleaning

- Identified missing values
- Removed duplicate records
- Validated feature formats and data quality

### 3. Exploratory Data Analysis (EDA)

- Analyzed target variable distribution
- Investigated numerical feature distributions
- Explored categorical variables
- Examined relationships between features and loan default status
- Visualized outliers using boxplots

### 4. Feature Engineering

A new feature was created:

```python
loan_percent_income = loan_amnt / person_income 

