# EconoCausal — Dynamic Pricing via Double Machine Learning

**Internship Project | Infotact Solutions**

## Project Overview

EconoCausal is a data science and causal machine learning project focused on analyzing marketing campaigns, coupon redemption, customer behavior, transaction data, and discount-related variables.

The objective is to investigate whether Double Machine Learning (DML) can support data-driven pricing decisions.

## Project Objectives

- Analyze marketing campaign and transaction data.
- Perform data quality checks.
- Validate relationships between datasets.
- Investigate customer coupon redemption behavior.
- Analyze customer demographics and coupon characteristics.
- Examine transaction prices and discount variables.
- Assess the feasibility of causal effect estimation.

## Dataset

This project uses the AmExpert 2019 Marketing Campaign dataset.

The dataset includes training and test data, campaign information, customer demographics, transaction records, coupon-item mappings, and item information.

Dataset source: https://www.kaggle.com/competitions/amexpert-2019/data

Raw dataset files are maintained locally and are not uploaded to this repository.

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
- Generated visualizations and CSV reports.

### Day 5 — Customer and Coupon Analysis
- Analyzed customer age ranges, marital status, and income brackets.
- Investigated missing demographic values.
- Examined product categories and brand types.
- Analyzed coupon-to-item relationships.
- Calculated observed redemption rates across demographic groups.
- Exported analysis results to CSV files.

### Day 6 — Transaction and Discount Analysis
- Inspected transaction columns, data types, and descriptive statistics.
- Examined selling prices, quantities, and discount variables.
- Investigated missing values and duplicate transaction rows.
- Analyzed customer transaction activity.
- Visualized coupon discount and other discount distributions.
- Examined correlations between numerical transaction variables.
- Exported four analysis reports to CSV files.

## Day 6 Outputs

- `day06_transaction_summary.csv`
- `day06_missing_values.csv`
- `day06_duplicate_analysis.csv`
- `day06_discount_correlation.csv`
- `DAY6_REPORT.md`

Notebook: `notebooks/06_transaction_discount_analysis.ipynb`

## Important Analytical Considerations

- The target variable is highly imbalanced, so accuracy alone may not be sufficient for evaluating future predictive models.
- Observed redemption rates and correlations do not establish causal effects.
- Missing demographic and transaction values require careful treatment.
- Duplicate records should not be removed automatically without understanding their meaning.
- Transaction-level discount values do not necessarily identify the discount treatment assigned to every customer.
- Causal modeling requires a defensible treatment definition, outcome, covariates, and identification assumptions.

## Next Steps

- Investigate relationships between transactions, coupons, campaigns, and redemption outcomes.
- Examine whether a suitable treatment variable can be defined.
- Assess whether the available data supports credible causal effect estimation.

---

**Current Status:** Day 6 transaction and discount analysis completed.
