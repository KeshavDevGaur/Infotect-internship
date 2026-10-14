# EconoCausal — Dynamic Pricing via Double Machine Learning

**Internship Project | Infotact Solutions**

## Project Overview

EconoCausal is a data science and causal machine learning project focused on analyzing marketing campaigns, coupon redemption, customer behavior, and discount-related variables.

The long-term objective is to investigate whether Double Machine Learning (DML) can support data-driven pricing decisions.

## Project Objectives

- Analyze marketing campaign and transaction data.
- Perform data quality checks.
- Validate relationships between datasets.
- Investigate customer coupon redemption behavior.
- Explore discount-related variables.
- Assess the feasibility of causal effect estimation.
- Build a reproducible machine learning workflow.

## Dataset

This project uses the AmExpert 2019 Marketing Campaign dataset.

The dataset includes:
- Training and test datasets.
- Campaign information.
- Customer demographic information.
- Customer transaction records.
- Coupon-to-item mappings.
- Product and item information.

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
- Loaded and inspected the available CSV files.
- Examined dataset dimensions and columns.
- Generated a dataset summary report.

### Day 2 — Data Quality Analysis
- Analyzed missing values.
- Checked duplicate records.
- Examined dataset quality issues.
- Validated basic dataset characteristics.

### Day 3 — Dataset Relationship Validation
- Checked campaign and coupon key coverage.
- Examined training dataset identifiers.
- Investigated customer demographic matching.
- Generated relationship validation reports.

### Day 4 — Target Variable and Campaign Analysis
- Analyzed the `redemption_status` target variable.
- Examined redemption and non-redemption counts.
- Calculated redemption rates for individual campaigns.
- Compared redemption rates across campaign types.
- Identified the top 10 campaigns by observed redemption rate.
- Created campaign performance visualizations.
- Exported analysis results to CSV files.

## Day 4 Outputs

The following reports were generated:

- `day04_campaign_redemption.csv`
- `day04_campaign_type_analysis.csv`
- `day04_top_campaigns.csv`
- `DAY4_REPORT.md`

Notebook: `04_target_analysis.ipynb`

## Repository Structure


EconoCausal/
├── README.md
├── .gitignore
├── requirements.txt
├── notebooks/
│   ├── README.md
│   ├── 01_data_inspection.ipynb
│   ├── 02_data_quality_analysis.ipynb
│   ├── 03_dataset_relationships.ipynb
│   └── 04_target_analysis.ipynb
└── reports/
    ├── README.md
    ├── DAY1_REPORT.md
    ├── DAY2_REPORT.md
    ├── DAY3_REPORT.md
    ├── DAY4_REPORT.md
    ├── day01_dataset_summary.csv
    ├── day02_duplicate_analysis.csv
    ├── day02_missing_values.csv
    ├── day03_relationship_validation.csv
    ├── day03_training_structure.csv
    ├── day04_campaign_redemption.csv
    ├── day04_campaign_type_analysis.csv
    └── day04_top_campaigns.csv
