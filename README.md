# Ecuadorian Credit Risk and Borrower Behavior Dataset

## Overview

This repository contains the documentation, metadata, data dictionary, quality reports, and reproducible preparation workflow for the **Ecuadorian Credit Risk and Borrower Behavior Dataset**.

The dataset contains **198,800 anonymized credit observations** from Ecuador’s cooperative and financial sector, covering consumer and microcredit products. It supports credit-risk research, including the prediction of adverse credit performance over a 12-month horizon, feature selection, temporal validation, and model explainability.

The dataset includes financial, delinquency, credit-exposure, contractual, and behavioral attributes derived from current and historical credit information.

## Dataset summary

- **Instances:** 198,800
- **Geographic scope:** Ecuador
- **Financial products:** Consumer credit and microcredit
- **Observation period:** 2024–2025
- **Observation frequency:** Quarterly
- **Available observation months:** January, April, July, and October
- **Dataset characteristics:** Tabular and multivariate
- **Primary task:** Binary classification
- **Primary target:** `performance_label_12m`
- **Missing values:** Yes
- **Language of variable names:** English
- **File encoding:** UTF-8
- **Missing-value representation:** Empty CSV fields

## Research purpose

The dataset was prepared to support reproducible academic and applied research on credit-risk modeling.

Potential research applications include:

- Prediction of adverse credit performance over a 12-month horizon
- Credit-risk classification
- Feature selection
- Model explainability
- Temporal model validation
- Missing-data treatment
- Algorithm comparison
- Class-imbalance analysis
- Model robustness
- Responsible machine learning in financial applications

The benchmark dataset is intended primarily for binary classification.

## Unit of observation

Each row represents an anonymized credit observation associated with a reported credit operation at a quarterly observation date.

An observation may contain information about:

- Credit product type
- Original operation amount
- Current balances
- Past-due balances
- Days past due
- Total debt exposure
- Legal-collection balances
- Charged-off balances
- Contractual timing
- Active and past-due operations
- Number of creditors
- Credit-card limits and utilization
- Historical credit behavior over different time windows

Direct borrower, operation, and reporting-institution identifiers are not included in the public files.

The public dataset should therefore be interpreted as a collection of anonymized credit observations rather than as an identifiable longitudinal record of individual borrowers.

## Dataset files

The preparation workflow produces the following files:

### Public release files

- `ecuador_credit_risk_full.csv`  
  Extended research file that retains credit-score attributes for explainability and score-comparison studies.

- `ecuador_credit_risk_data_dictionary.csv`  
  Public dictionary containing attribute roles, data types, units, time windows, missingness, definition status, descriptions, and benchmark inclusion.


## Target variable

The primary target is:

```text
performance_label_12m
