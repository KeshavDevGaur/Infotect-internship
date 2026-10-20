# EconoCausal — Dynamic Pricing via Double Machine Learning

### Internship Project | Infotact Solutions

## 📌 Project Overview

EconoCausal is a data analysis and causal inference project focused on marketing campaigns, coupon redemption, customer demographics, and transaction discounts.

The project uses the AmExpert 2019 Marketing Campaign dataset to explore customer behavior, validate relationships between datasets, and investigate whether the available data can support a defensible causal analysis.

The long-term objective is to assess whether Double Machine Learning (DML) can be applied to estimate a meaningful causal effect, provided that the treatment, outcome, covariates, and identification assumptions can be established.

## 🎯 Project Objectives

- Understand the structure of the available datasets.
- Identify missing values, duplicate records, and data-quality issues.
- Validate relationships between related datasets.
- Analyze coupon redemption patterns across campaigns.
- Investigate customer demographics and coupon-item relationships.
- Explore transaction and discount information.
- Integrate datasets while validating join relationships.
- Investigate potential treatment and outcome variables.
- Analyze campaign distributions and redemption rates.
- Assess whether campaign exposure can be established.
- Evaluate the feasibility of causal inference before modeling.

## 📊 Dataset Information

**Dataset:** AmExpert 2019 Marketing Campaign

**Source:** [Kaggle — AmExpert 2019 Marketing Campaign](https://www.kaggle.com/competitions/amexpert-2019/data)

### Datasets Used

| Dataset | Description |
|---|---|
| `train.csv` | Training data containing customer, campaign, coupon, and redemption information |
| `test_QyjYwdj.csv` | Test dataset for the original competition |
| `campaign_data.csv` | Campaign-related information |
| `customer_demographics.csv` | Customer demographic information |
| `customer_transaction_data.csv` | Historical customer transaction records |
| `coupon_item_mapping.csv` | Mapping between coupons and items |
| `item_data.csv` | Item-related information |
| `sample_submission_Byiv0dS.csv` | Sample submission format for the original competition |

**Note:** Raw datasets are excluded from Git version control.

## 🛠️ Technology Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- JupyterLab
- GitHub
- Double Machine Learning (potential future method)

## 📁 Project Structure

```text
Infotect-internship/
├── README.md
└── EconoCausal/
    ├── .gitignore
    ├── requirements.txt
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
    │   └── 09_campaign_exposure_analysis.ipynb
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
        ├── day01_dataset_summary.csv
        ├── day02_duplicate_analysis.csv
        ├── day02_missing_values.csv
        ├── day03_relationship_validation.csv
        ├── day03_training_structure.csv
        ├── day04_campaign_redemption.csv
        ├── day04_campaign_type_analysis.csv
        ├── day04_top_campaigns.csv
        ├── day05_age_redemption.csv
        ├── day05_marital_redemption.csv
        ├── day05_income_redemption.csv
        ├── day05_coupon_item_counts.csv
        ├── day05_category_counts.csv
        ├── day06_transaction_summary.csv
        ├── day06_missing_values.csv
        ├── day06_duplicate_analysis.csv
        ├── day06_discount_correlation.csv
        ├── day07_integration_summary.csv
        ├── day07_causal_variable_summary.csv
        ├── day08_causal_assessment.csv
        ├── day09_campaign_counts.csv
        └── day09_campaign_redemption.csv
```

*This structure describes the intended organization. Ensure filenames match the files actually committed to GitHub.*

## 📅 Development Progress

| Day | Work Completed | Status |
|---|---|---|
| Day 1 | Dataset inspection and initial project setup | Completed |
| Day 2 | Missing-value and duplicate analysis | Completed |
| Day 3 | Dataset relationship validation | Completed |
| Day 4 | Target distribution and campaign analysis | Completed |
| Day 5 | Customer demographics and coupon-item analysis | Completed |
| Day 6 | Transaction and discount analysis | Completed |
| Day 7 | Dataset integration and causal-variable investigation | Completed |
| Day 8 | Preliminary treatment and outcome assessment | Completed |
| Day 9 | Campaign distribution, redemption analysis, and exposure investigation | Completed |

## 🔍 Work Completed

### Day 1 — Dataset Inspection

- Loaded and inspected the available datasets.
- Examined dataset dimensions and columns.
- Generated a dataset summary.
- Established the initial project structure.

**Output:** `day01_dataset_summary.csv`

### Day 2 — Data Quality Analysis

- Investigated missing values.
- Identified duplicate records.
- Examined potential data-quality issues.

**Outputs:**
- `day02_missing_values.csv`
- `day02_duplicate_analysis.csv`

### Day 3 — Dataset Relationship Validation

- Examined potential join keys.
- Validated relationships between datasets.
- Investigated unmatched records.
- Documented the training dataset structure.

**Outputs:**
- `day03_relationship_validation.csv`
- `day03_training_structure.csv`

### Day 4 — Target and Campaign Analysis

- Analyzed the distribution of `redemption_status`.
- Investigated campaign-level redemption patterns.
- Compared campaign types.
- Identified campaigns with higher observed redemption rates.

**Outputs:**
- `day04_campaign_redemption.csv`
- `day04_campaign_type_analysis.csv`
- `day04_top_campaigns.csv`

### Day 5 — Customer and Coupon Analysis

- Examined customer demographic characteristics.
- Investigated redemption patterns across age groups.
- Analyzed marital-status and income-related patterns.
- Examined coupon-item mappings and item categories.

**Outputs:**
- `day05_age_redemption.csv`
- `day05_marital_redemption.csv`
- `day05_income_redemption.csv`
- `day05_coupon_item_counts.csv`
- `day05_category_counts.csv`

### Day 6 — Transaction and Discount Analysis

- Inspected historical transaction records.
- Examined transaction discount variables.
- Investigated duplicate transaction records.
- Reviewed missing values and discount correlations.
- Documented considerations for interpreting transaction data.

**Outputs:**
- `day06_transaction_summary.csv`
- `day06_missing_values.csv`
- `day06_duplicate_analysis.csv`
- `day06_discount_correlation.csv`

### Day 7 — Dataset Integration

- Integrated training records with campaign information.
- Integrated customer demographic information.
- Connected coupon-item mappings with item information.
- Connected transaction records with customer demographics.
- Validated merge relationships and row preservation.
- Investigated variables potentially relevant to causal analysis.

**Outputs:**
- `day07_integration_summary.csv`
- `day07_causal_variable_summary.csv`

### Day 8 — Treatment and Outcome Assessment

- Inspected potential treatment and outcome variables.
- Investigated discount-related columns.
- Examined the redemption outcome distribution.
- Inspected campaign characteristics.
- Prepared a preliminary causal-variable assessment.
- Documented uncertainties regarding treatment assignment.

**Outputs:**
- `day08_causal_assessment.csv`
- `DAY8_REPORT.md`

### Day 9 — Campaign Exposure Analysis

- Analyzed the number of training records per campaign.
- Counted unique coupons and customers per campaign.
- Calculated campaign-level redemption counts and rates.
- Inspected training and campaign dataset columns.
- Investigated customer demographic coverage.
- Examined whether the available columns establish campaign exposure.
- Exported campaign analysis summaries.

**Outputs:**
- `day09_campaign_counts.csv`
- `day09_campaign_redemption.csv`
- `DAY9_REPORT.md`

## 📈 Key Observations

- Coupon redemption is a rare event in the training dataset.
- Some customer demographic fields contain substantial missing values.
- Dataset integration requires careful validation of join keys and relationship cardinality.
- A coupon can map to multiple items, so coupon-item joins can increase row counts.
- Campaigns may differ in record counts, coupon counts, customer counts, and observed redemption rates.
- Customer demographic data does not necessarily cover every customer in the training dataset.
- Recorded transaction discounts do not automatically represent assigned treatments.
- Campaign identifiers alone do not establish randomized assignment or prove customer exposure.
- Differences in observed redemption rates do not, by themselves, demonstrate causal effects.

## 🧠 Causal Inference Preparation

The project investigates whether Double Machine Learning (DML) is appropriate for the available data.

Before estimating a causal effect, the following must be established:

### 1. Treatment

A clearly defined intervention or exposure whose effect can be evaluated.

### 2. Outcome

A measurable result associated with the research question. The training dataset contains `redemption_status`, an observed coupon redemption outcome.

### 3. Covariates

Relevant pre-treatment characteristics that may help account for confounding.

### 4. Identification Assumptions

A defensible explanation of why the available data can identify the intended causal effect.

### 5. Data Suitability

Sufficient information to define treatment exposure, compare relevant conditions, and evaluate possible sources of bias.

**Important:** The treatment definition remains under investigation. Recorded transaction discounts have not been established as treatment assignments for all customers. No causal effect should be claimed without a defensible identification strategy.

## 📂 Project Documentation

- `notebooks/` — Jupyter notebooks containing analysis code.
- `reports/` — Daily reports and exported CSV summaries.
- `data/raw/` — Local raw datasets, excluded from version control.

## 🚀 Next Steps

- Investigate the relationship between campaign assignments, coupons, customers, and redemption records.
- Determine whether campaign exposure can be established reliably.
- Evaluate whether a defensible treatment and comparison group can be defined.
- Identify suitable pre-treatment covariates.
- Investigate potential confounding and selection bias.
- Document the limitations of the available observational data.
- Select an appropriate causal estimation strategy only if the data supports the research question.
- Implement and evaluate a causal model if the required assumptions and data are defensible.

## 👨‍💻 Project Information

- **Project Name:** EconoCausal
- **Organization:** Infotact Solutions
- **Domain:** Data Science and Causal Inference
- **Primary Language:** Python
- **Dataset:** AmExpert 2019 Marketing Campaign
- **Progress:** Days 1–9 completed

---

*This project emphasizes reproducible analysis, data validation, transparent assumptions, and responsible interpretation of results.*
