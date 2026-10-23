# EconoCausal — Reports and Analysis Outputs

This directory contains daily progress reports and CSV analysis outputs for the **EconoCausal — Dynamic Pricing via Double Machine Learning** project developed during the Infotact Solutions internship.

The reports document dataset inspection, data-quality checks, campaign analysis, customer behavior, transaction patterns, dataset integration, and preliminary causal analysis.

## 📅 Daily Report Index

| Day | Report            | Description                                                | Status    |
| --- | ----------------- | ---------------------------------------------------------- | --------- |
| 1   | `DAY1_REPORT.md`  | Dataset inspection and initial summary                     | Completed |
| 2   | `DAY2_REPORT.md`  | Missing values and duplicate analysis                      | Completed |
| 3   | `DAY3_REPORT.md`  | Dataset relationships and identifier validation            | Completed |
| 4   | `DAY4_REPORT.md`  | Target distribution and campaign analysis                  | Completed |
| 5   | `DAY5_REPORT.md`  | Customer demographics and coupon-item analysis             | Completed |
| 6   | `DAY6_REPORT.md`  | Transaction and discount analysis                          | Completed |
| 7   | `DAY7_REPORT.md`  | Dataset integration and causal-variable investigation      | Completed |
| 8   | `DAY8_REPORT.md`  | Preliminary treatment and outcome assessment               | Completed |
| 9   | `DAY9_REPORT.md`  | Campaign distribution and exposure investigation           | Completed |
| 10  | `DAY10_REPORT.md` | Customer-campaign relationships and coupon distribution    | Completed |
| 11  | `DAY11_REPORT.md` | Treatment, outcome, and covariate assessment               | Completed |
| 12  | `DAY12_REPORT.md` | Treatment assignment and causal identification feasibility | Completed |

## 📊 CSV Analysis Outputs

### Day 1 — Dataset Inspection

* `day01_dataset_summary.csv`

**Purpose:** Summarizes the available datasets, including their dimensions and basic structure.

### Day 2 — Data Quality Analysis

* `day02_missing_values.csv`
* `day02_duplicate_analysis.csv`

**Purpose:** Documents missing values and duplicate records to help assess data quality.

### Day 3 — Dataset Relationship Validation

* `day03_relationship_validation.csv`
* `day03_training_structure.csv`

**Purpose:** Records relationship-validation results, key coverage, and training dataset structure.

### Day 4 — Target and Campaign Analysis

* `day04_campaign_redemption.csv`
* `day04_campaign_type_analysis.csv`
* `day04_top_campaigns.csv`

**Purpose:** Summarizes redemption patterns, campaign-type comparisons, and campaigns with high observed redemption rates.

### Day 5 — Customer and Coupon Analysis

* `day05_age_redemption.csv`
* `day05_marital_redemption.csv`
* `day05_income_redemption.csv`
* `day05_coupon_item_counts.csv`
* `day05_category_counts.csv`

**Purpose:** Documents demographic redemption patterns, coupon-item relationships, and item-category distributions.

### Day 6 — Transaction and Discount Analysis

* `day06_transaction_summary.csv`
* `day06_missing_values.csv`
* `day06_duplicate_analysis.csv`
* `day06_discount_correlation.csv`

**Purpose:** Summarizes transaction activity, missing values, duplicates, and observed relationships involving discount variables.

### Day 7 — Dataset Integration

* `day07_integration_summary.csv`
* `day07_causal_variable_summary.csv`

**Purpose:** Records dataset integration results, merge validation, and an initial assessment of variables that may be relevant to causal analysis.

### Day 8 — Treatment and Outcome Assessment

* `day08_causal_assessment.csv`

**Purpose:** Documents the preliminary assessment of potential treatment variables, outcome variables, and limitations in the available data.

### Day 9 — Campaign Exposure Analysis

* `day09_campaign_counts.csv`
* `day09_campaign_redemption.csv`

**Purpose:** Summarizes campaign-level record counts, customer and coupon coverage, and observed redemption rates.

### Day 10 — Customer-Campaign Relationship Analysis

* `day10_customer_campaign_counts.csv`
* `day10_campaign_coupon_summary.csv`
* `day10_coupon_campaign_counts.csv`
* `day10_relationship_validation.csv`

**Purpose:** Documents customer-campaign relationships, coupon distribution across campaigns, duplicate-combination checks, and identifier validation.

### Day 11 — Treatment and Outcome Definition

* `day11_treatment_outcome_assessment.csv`

**Purpose:** Documents the preliminary assessment of the outcome variable, potential treatment, possible covariates, identifiers, and unresolved causal-analysis requirements.

### Day 12 — Treatment Assignment Analysis

* `day12_treatment_assignment_assessment.csv`

**Purpose:** Documents campaign metadata findings, potential evidence of treatment assignment, and unresolved questions about customer-level exposure and causal identification.

## 🎯 Project Objectives

The reporting workflow supports the following objectives:

1. Understand the structure and quality of the available data.
2. Explore customer, coupon, campaign, and transaction relationships.
3. Investigate observed coupon-redemption patterns.
4. Identify potential treatment, outcome, and covariate variables.
5. Evaluate whether the available data can support a defensible causal analysis.
6. Maintain reproducible analysis records and daily internship documentation.

## ⚠️ Causal Analysis Limitations

The current reports primarily document exploratory data analysis and preliminary causal feasibility.

Important distinctions must be maintained:

* Observed coupon redemption does not, by itself, establish the causal effect of a discount.
* A campaign identifier does not necessarily prove that a customer was exposed to a campaign.
* Campaign dates do not independently establish customer-level treatment assignment.
* Transaction discount records do not automatically establish treatment assignment.
* Differences in redemption rates across campaigns or customer groups may reflect confounding factors.
* A valid Double Machine Learning analysis requires a clearly defined treatment, outcome, suitable pre-treatment covariates, and defensible identification assumptions.

Consequently, no causal effect should be claimed until the treatment definition, data structure, and identification strategy have been adequately established.

## 📁 Directory Structure

```text
EconoCausal/
├── notebooks/
│   ├── README.md
│   ├── 01_data_inspection.ipynb
│   ├── 02_data_quality_analysis.ipynb
│   ├── 03_dataset_relationships.ipynb
│   ├── 04_target_analysis.ipynb
│   ├── 05_customer_coupon_analysis.ipynb
│   ├── 06_transaction_discount_analysis.ipynb
│   ├── 07_dataset_integration.ipynb
│   ├── 08_treatment_outcome_analysis.ipynb
│   ├── 09_campaign_exposure_analysis.ipynb
│   ├── 10_customer_campaign_relationships.ipynb
│   ├── 11_treatment_outcome_definition.ipynb
│   └── 12_treatment_assignment_analysis.ipynb
│
└── reports/
    ├── README.md
    ├── DAY1_REPORT.md
    ├── DAY2_REPORT.md
    ├── DAY3_REPORT.md
    ├── DAY4_REPORT.md
    ├── DAY5_REPORT.md
    ├── DAY6_REPORT.md
    ├── DAY7_REPORT.md
    ├── DAY8_REPORT.md
    ├── DAY9_REPORT.md
    ├── DAY10_REPORT.md
    ├── DAY11_REPORT.md
    ├── DAY12_REPORT.md
    └── day12_treatment_assignment_assessment.csv
```

*This directory structure represents the intended organization. Ensure that each listed file exists in the repository before considering the documentation complete.*

## 🛠️ Tools and Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* JupyterLab
* GitHub

## 📌 Project Information

* **Project Name:** EconoCausal — Dynamic Pricing via Double Machine Learning
* **Organization:** Infotact Solutions
* **Domain:** Data Science and Causal Inference
* **Documentation Progress:** Days 1–12

---

*Reports and CSV outputs are maintained to support reproducibility, transparent data analysis, and progress tracking throughout the internship.*
