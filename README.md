# EconoCausal — Dynamic Pricing via Double Machine Learning

**Internship Project | Infotact Solutions**

## Project Overview

EconoCausal is a data science and causal machine learning project focused on analyzing marketing campaigns, coupon redemption, customer behavior, and discount-related variables.

The objective is to investigate whether Double Machine Learning (DML) can support data-driven pricing decisions.

## Project Objectives

- Analyze marketing campaign and transaction data.
- Perform data quality checks.
- Validate relationships between datasets.
- Investigate customer coupon redemption behavior.
- Explore customer demographics and coupon characteristics.
- Assess the feasibility of causal effect estimation.

## Dataset

This project uses the AmExpert 2019 Marketing Campaign dataset.

The dataset includes training and test data, campaign information, customer demographics, transaction records, coupon-item mappings, and item information.

Dataset source: https://www.kaggle.com/competitions/amexpert-2019/data

Raw datasets are maintained locally and are not uploaded to this repository.

## Technology Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- JupyterLab
- GitHub

## Project Progress

### Day 1 — Dataset Inspection
- Loaded and inspected the available datasets.
- Examined dataset dimensions and columns.
- Generated a dataset summary report.

### Day 2 — Data Quality Analysis
- Analyzed missing values.
- Checked duplicate records.
- Investigated data quality issues.

### Day 3 — Dataset Relationship Validation
- Checked campaign and coupon key coverage.
- Examined training dataset identifiers.
- Investigated customer demographic matching.

### Day 4 — Target Variable and Campaign Analysis
- Analyzed the `redemption_status` target variable.
- Calculated campaign-level redemption rates.
- Compared redemption rates across campaign types.
- Identified the top 10 campaigns by observed redemption rate.
- Created visualizations and CSV reports.

### Day 5 — Customer and Coupon Analysis
- Analyzed customer age ranges, marital status, and income brackets.
- Investigated missing demographic values.
- Examined product categories and brand types.
- Analyzed coupon-to-item relationships.
- Calculated observed redemption rates by age group.
- Compared redemption rates by marital status and income bracket.
- Exported five analysis reports to CSV.

## Day 5 Outputs

- `day05_age_redemption.csv`
- `day05_marital_redemption.csv`
- `day05_income_redemption.csv`
- `day05_coupon_item_counts.csv`
- `day05_category_counts.csv`
- `DAY5_REPORT.md`

Notebook: `notebooks/05_customer_coupon_analysis.ipynb`

## Important Analytical Considerations

- The target variable is highly imbalanced, so accuracy alone may not be sufficient for evaluating future predictive models.
- Observed redemption rates do not establish causal effects.
- Missing demographic information requires careful handling.
- Transaction discount values do not automatically establish the treatment assigned to every customer.
- Causal modeling requires a defensible treatment definition, outcome, covariates, and identification assumptions.

## Next Steps

- Investigate transaction behavior and discount-related variables.
- Examine relationships between campaigns, coupons, customers, and transactions.
- Assess whether the data supports credible causal effect estimation.

---

**Current Status:** Day 5 analysis completed.
