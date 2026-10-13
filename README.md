# EconoCausal: Dynamic Pricing via Double Machine Learning

## Project Overview

EconoCausal investigates retail promotional campaigns and customer purchasing behavior, with the long-term goal of evaluating causal effects relevant to dynamic pricing.

The project uses the AmExpert 2019 Marketing Campaign dataset.

## Project Progress

### Day 1 — Dataset Inspection
- Loaded and inspected the available CSV datasets.
- Recorded dataset dimensions and initial data-quality statistics.
- Generated the initial dataset summary.

### Day 2 — Data Quality Analysis
- Investigated missing values.
- Examined duplicate records.
- Generated missing-value and duplicate-analysis reports.

### Day 3 — Dataset Relationship Validation
- Checked relationships between training records and campaign data.
- Validated training coupon identifiers against coupon-item mapping.
- Checked customer demographic coverage.
- Verified training record identifiers and uniqueness.
- Generated relationship-validation and training-structure reports.

## Key Findings

- Training records: 78,369
- Unique training IDs: 78,369
- Unique campaigns in training: 18
- Unique coupons in training: 866
- Unique customers in training: 1,428
- Duplicate training IDs: 0
- Training records matching customer demographics: 55.71%
- Training records without demographic matches: 44.29%

These findings describe the checks completed so far. They do not establish a causal effect or confirm that the dataset contains all the treatment information required for causal pricing.

## Repository Structure

```text
EconoCausal/
├── notebooks/
│   ├── 01_data_inspection.ipynb
│   ├── 02_data_quality_analysis.ipynb
│   ├── 03_dataset_relationships.ipynb
│   └── README.md
├── reports/
│   ├── DAY1_REPORT.md
│   ├── DAY2_REPORT.md
│   ├── DAY3_REPORT.md
│   ├── day01_dataset_summary.csv
│   ├── day02_duplicate_analysis.csv
│   ├── day02_missing_values.csv
│   ├── day03_relationship_validation.csv
│   ├── day03_training_structure.csv
│   └── README.md
├── .gitignore
├── requirements.txt
└── README.md
