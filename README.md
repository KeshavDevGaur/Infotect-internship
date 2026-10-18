# EconoCausal — Dynamic Pricing via Double Machine Learning

### Internship Project | Infotact Solutions

## 📌 Project Overview

**EconoCausal** is a data analysis and causal inference project that investigates marketing campaigns, coupon redemption, customer demographics, and transaction discounts.

The project uses the **AmExpert 2019 Marketing Campaign dataset** to explore customer behavior, validate relationships between datasets, and investigate whether the available data can support a defensible causal analysis.

The long-term objective is to assess whether **Double Machine Learning (DML)** can be applied to estimate a meaningful causal effect. This requires establishing a valid treatment variable, outcome, covariates, and identification assumptions before performing causal estimation.

## 🎯 Project Objectives

- Understand the structure of the available datasets.
- Identify missing values, duplicate records, and data-quality issues.
- Validate relationships between related datasets.
- Analyze coupon redemption patterns across campaigns.
- Investigate customer demographics and coupon-item relationships.
- Explore transaction and discount information.
- Integrate related datasets while validating row counts.
- Assess the feasibility of causal inference.
- Prepare the data for subsequent modeling and evaluation.

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

### Important Dataset Considerations

- The training target is `redemption_status`.
- The target is highly imbalanced, with approximately 0.93% positive redemption records in the initial analysis.
- Some demographic fields contain substantial missing values.
- Customer and coupon relationships must be validated before merging datasets.
- Recorded transaction discounts do not automatically establish which discount treatment was assigned to each customer.
- Raw datasets are excluded from Git version control.

## 🛠️ Technology Stack

- **Programming Language:** Python
- **Data Manipulation:** Pandas, NumPy
- **Data Visualization:** Matplotlib, Seaborn
- **Development Environment:** JupyterLab / Jupyter Notebook
- **Version Control:** GitHub
- **Potential Future Method:** Double Machine Learning (DML)

## 📁 Project Structure

```text
Infotect-internship/
├── README.md
└── EconoCausal/
    ├── .gitignore
    ├── requirements.txt
    │
    ├── notebooks/
    │   ├── README.md
    │   ├── 01_data_inspection.ipynb
    │   ├── 02_data_quality_analysis.ipynb
    │   ├── 03_dataset_relationships.ipynb
    │   ├── 04_target_analysis.ipynb
    │   ├── 05_customer_coupon_analysis.ipynb
    │   ├── 06_transaction_discount_analysis.ipynb
    │   └── 07_dataset_integration.ipynb
    │   └── 08_treatment_outcome_analysis.ipynb
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
        └── day07_causal_variable_summary.csv
        └── day08_causal_assessment.csv
```

*Note: This structure documents the intended project layout. It should match the files actually committed to the repository.*

## 📅 Development Progress

### Day 1 — Dataset Inspection
- Loaded and inspected the available datasets.
- Reviewed dataset dimensions and columns.
- Generated a dataset summary.
- Established the initial project structure.

**Output:** `day01_dataset_summary.csv`

### Day 2 — Data Quality Analysis
- Investigated missing values.
- Identified duplicate records.
- Examined potential data-quality issues.
- Exported missing-value and duplicate summaries.

**Outputs:**
- `day02_missing_values.csv`
- `day02_duplicate_analysis.csv`

### Day 3 — Dataset Relationship Validation
- Examined potential join keys.
- Validated relationships between the training data and related datasets.
- Investigated unmatched records.
- Documented the training dataset structure.

**Outputs:**
- `day03_relationship_validation.csv`
- `day03_training_structure.csv`

### Day 4 — Target and Campaign Analysis
- Analyzed the distribution of `redemption_status`.
- Investigated redemption patterns across campaigns.
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

### Day 7 — Dataset Integration and Causal Feasibility
- Integrated training records with campaign information.
- Integrated customer demographic information with training records.
- Connected coupon-item mappings with item information.
- Integrated transaction records with customer demographics.
- Validated merge relationships and row preservation.
- Inspected variables potentially relevant to causal analysis.
- Documented uncertainties concerning treatment definition.

**Outputs:**
- `day07_integration_summary.csv`
- `day07_causal_variable_summary.csv`

### Day 8 — Treatment and Outcome Definition
- Loaded training, transaction, campaign, and customer demographic datasets.
- Inspected columns to identify potential treatment and outcome variables.
- Investigated discount-related variables and their distributions.
- Examined the distribution of the `redemption_status` outcome.
- Checked the availability of outcome and potential treatment-related variables.
- Inspected campaign information and campaign characteristics.
- Created a preliminary causal variable assessment.
- Documented uncertainties regarding treatment assignment and causal feasibility.

**Outputs:**

- `day08_causal_assessment.csv`
- `DAY8_REPORT.md`
- `08_treatment_outcome_analysis.ipynb`

**Status:** Days 1–8 completed.

## 🔍 Key Observations

- Coupon redemption is a rare event in the training dataset.
- Missing demographic information may affect feature selection and analysis.
- Related datasets have different levels of detail and must be joined carefully.
- A coupon may map to multiple items, so coupon-item joins can increase row counts.
- Left joins can preserve records while leaving unmatched information missing.
- Transaction-level discount values should not automatically be interpreted as assigned treatments.
- Observational associations do not, by themselves, establish causal effects.

## 🧠 Causal Inference Approach

The project investigates the potential application of **Double Machine Learning (DML)**.

Before estimating any causal effect, the following must be established:

1. **Treatment:** A clearly defined intervention or exposure with a defensible interpretation.
2. **Outcome:** A measurable result associated with the research question.
3. **Covariates:** Relevant pre-treatment variables used to account for confounding.
4. **Identification assumptions:** A defensible explanation of why the observed data can identify the causal effect.
5. **Data validation:** Confirmation that the required variables and relationships exist and are suitable for the analysis.

The observed `redemption_status` is an outcome in the training data. However, the available transaction discount columns have not yet been established as valid treatment assignments.

**No causal effect should be claimed until the treatment definition, data limitations, and identification assumptions have been carefully evaluated.**

## 🚀 Upcoming Work

The next stages will focus on:

- Investigating the relationship between campaign assignment, coupon redemption, and transaction records.
- Determining whether a defensible treatment and outcome can be constructed.
- Identifying suitable pre-treatment covariates.
- Assessing confounding, selection bias, and data limitations.
- Selecting an appropriate estimation strategy based on the evidence.
- Implementing and evaluating a causal model only if the data supports it.
- Documenting findings, assumptions, and limitations.

## 📂 Reports and Notebooks

Detailed daily analyses are maintained in the `notebooks/` and `reports/` directories.

- **Notebooks:** Analysis code and results.
- **Reports:** Daily progress summaries and exported CSV results.
- **Raw data:** Stored locally and excluded from version control.

## 👨‍💻 Project Information

- **Project Name:** EconoCausal
- **Organization:** Infotact Solutions
- **Domain:** Data Science and Causal Inference
- **Primary Language:** Python
- **Dataset:** AmExpert 2019 Marketing Campaign

---

*This project is being developed iteratively, with an emphasis on reproducible analysis, data validation, transparent assumptions, and responsible interpretation of results.*
