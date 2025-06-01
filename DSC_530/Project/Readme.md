# Credit Risk Analysis

## Project Overview

This project is part of  ** Data Exploration and Analysis**, focusing on understanding and modeling **credit risk** through data analysis techniques. The goal is to identify and interpret the factors influencing loan approvals using exploratory data analysis (EDA), statistical modeling, and hypothesis testing.

## Dataset

The project utilizes the `credit_risk_dataset`, which includes several relevant features for analyzing credit risk:

- **person_age**: Age of the loan applicant
- **person_income**: Income level of the applicant
- **person_home_ownership**: Type of home ownership (e.g., rent, own)
- **person_emp_length**: Employment length in years
- **loan_intent**: Purpose of the loan (e.g., education, medical)
- **loan_grade**: Assigned credit grade
- **loan_amnt**: Loan amount requested
- **loan_int_rate**: Interest rate applied
- **loan_status**: Whether the loan was approved (target variable)
- **cb_person_default_on_file**: Default history of the applicant
- **cb_person_cred_hist_length**: Credit history length in years

## Objectives

The analysis covers the following aspects:

- Perform data cleaning and preprocessing
- Conduct descriptive statistics (mean, median, mode, histograms)
- Analyze distributions using PMF and CDF
- Fit analytical distributions and interpret fit
- Explore relationships using scatter plots and correlation analysis
- Test hypotheses with appropriate statistical methods
- Conduct regression analysis for predictive modeling

## Key Tasks

- Handle missing values and clean extreme outliers (e.g., age > 85)
- Visualize distributions and identify skewness or outliers
- Calculate and interpret Pearson correlation coefficients
- Compare PMF and CDF across scenarios (e.g., loan intent)
- Perform regression analysis on variables like income, intent, and interest rate
- Evaluate the predictive power and assumptions of the regression model

## Summary

This notebook culminates in a comprehensive credit risk assessment, blending descriptive, inferential, and predictive analytics. The insights derived aim to support decision-making in loan approval processes.

## Requirements

To run this notebook, ensure the following Python libraries are installed:

```bash
pandas
numpy
matplotlib
seaborn
scipy
sklearn
```

## Usage

Open the notebook using Jupyter Notebook or JupyterLab and run each cell sequentially to reproduce the analysis.
