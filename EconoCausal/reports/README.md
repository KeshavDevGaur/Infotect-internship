# EconoCausal — Reports and Analysis Outputs

This directory contains daily progress reports and CSV outputs generated during the development of the EconoCausal internship project at Infotact Solutions.

The reports document dataset inspection, data quality analysis, campaign redemption, customer behavior, transaction analysis, and dataset integration.

## Daily Progress Reports

| Day | Report | Description | Status |
|---|---|---|---|
| 1 | `DAY1_REPORT.md` | Dataset inspection and initial project setup | Completed |
| 2 | `DAY2_REPORT.md` | Missing values and duplicate analysis | Completed |
| 3 | `DAY3_REPORT.md` | Dataset relationships and join validation | Completed |
| 4 | `DAY4_REPORT.md` | Target distribution and campaign analysis | Completed |
| 5 | `DAY5_REPORT.md` | Customer demographics and coupon-item analysis | Completed |
| 6 | `DAY6_REPORT.md` | Transaction and discount analysis | Completed |
| 7 | `DAY7_REPORT.md` | Dataset integration and causal feasibility investigation | Completed |
| 8 | `DAY7_REPORT.md` | Preliminary treatment and outcome assessment, discount investigation, and causal feasibility | Completed |

## CSV Analysis Outputs

### Day 1 — Dataset Inspection
- `day01_dataset_summary.csv`

### Day 2 — Data Quality Analysis
- `day02_missing_values.csv`
- `day02_duplicate_analysis.csv`

### Day 3 — Dataset Relationship Validation
- `day03_relationship_validation.csv`
- `day03_training_structure.csv`

### Day 4 — Campaign and Target Analysis
- `day04_campaign_redemption.csv`
- `day04_campaign_type_analysis.csv`
- `day04_top_campaigns.csv`

### Day 5 — Customer and Coupon Analysis
- `day05_age_redemption.csv`
- `day05_marital_redemption.csv`
- `day05_income_redemption.csv`
- `day05_coupon_item_counts.csv`
- `day05_category_counts.csv`

### Day 6 — Transaction and Discount Analysis
- `day06_transaction_summary.csv`
- `day06_missing_values.csv`
- `day06_duplicate_analysis.csv`
- `day06_discount_correlation.csv`

### Day 7 — Dataset Integration and Causal Variables
- `day07_integration_summary.csv`
- `day07_causal_variable_summary.csv`

### Day 8 — Treatment and Outcome Assessment
- `DAY8_REPORT.md` — Documents the preliminary treatment and outcome investigation.
- `day08_causal_assessment.csv` — Summarizes candidate treatment, outcome, identifier, and covariate variables.


## Purpose of These Reports

The reports and CSV files support:

- Reproducible data exploration
- Data-quality assessment
- Validation of dataset relationships
- Investigation of campaign and redemption patterns
- Documentation of missing values and duplicate records
- Evaluation of potential variables for causal analysis

## Important Causal Analysis Consideration

The presence of transaction discount variables does not automatically establish a valid treatment variable.

Before applying Double Machine Learning, the project must define a defensible treatment, outcome, covariates, and identification assumptions. Observational correlations alone do not demonstrate causal effects.

## Related Project Files

- Analysis notebooks are stored in `../notebooks/`.
- Project documentation is maintained in the parent `EconoCausal/` directory.
- Raw datasets are excluded from version control.

---

**Project:** EconoCausal — Dynamic Pricing via Double Machine Learning  
**Organization:** Infotact Solutions  
**Progress:** Days 1–8 completed
