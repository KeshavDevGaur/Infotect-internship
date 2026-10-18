# EconoCausal — Notebooks

This directory contains the Jupyter notebooks developed for the EconoCausal internship project at Infotact Solutions.

The notebooks document dataset inspection, data quality checks, campaign analysis, customer behavior, transaction discounts, and dataset integration.

## Notebook Index

| Day | Notebook | Description | Status |
|---|---|---|---|
| 1 | `01_data_inspection.ipynb` | Initial dataset inspection, dimensions, columns, and summary statistics | Completed |
| 2 | `02_data_quality_analysis.ipynb` | Missing values, duplicate records, and data quality | Completed |
| 3 | `03_dataset_relationships.ipynb` | Join keys, dataset relationships, and unmatched records | Completed |
| 4 | `04_target_analysis.ipynb` | Redemption distribution and campaign-level analysis | Completed |
| 5 | `05_customer_coupon_analysis.ipynb` | Customer demographics, coupon-item mappings, and category analysis | Completed |
| 6 | `06_transaction_discount_analysis.ipynb` | Transaction patterns, discount variables, missing values, and duplicates | Completed |
| 7 | `07_dataset_integration.ipynb` | Dataset integration, merge validation, and causal-variable investigation | Completed |
| 8 | `08_treatment_outcome_analysis.ipynb` | Preliminary treatment and outcome assessment, discount investigation, and causal feasibility | Completed |

## Topics Covered

### Data Inspection and Quality
- Dataset dimensions and column inspection
- Missing-value analysis
- Duplicate detection
- Key uniqueness and relationship validation

### Exploratory Data Analysis
- Target distribution
- Campaign redemption patterns
- Customer demographic analysis
- Coupon-item mapping analysis
- Transaction and discount exploration

### Dataset Integration
- Merging training records with campaign information
- Integrating customer demographics
- Connecting coupon mappings with item information
- Connecting transactions with customer demographics
- Checking row preservation and unmatched records

### Causal Analysis Preparation
- Identifying potential treatment and outcome variables
- Inspecting candidate covariates
- Investigating data limitations
- Evaluating whether causal estimation is defensible

## Outputs

Analysis summaries and daily reports are stored in the `../reports/` directory.

## Important Note

Observed correlations and redemption patterns do not establish causal effects. Treatment definition, outcome selection, covariates, and identification assumptions must be evaluated before applying Double Machine Learning.

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- JupyterLab

---

**Project:** EconoCausal — Dynamic Pricing via Double Machine Learning  
**Organization:** Infotact Solutions
