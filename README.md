# EconoCausal — Dynamic Pricing via Double Machine Learning

**Internship Project | Infotact Solutions | Data Science & Causal Inference**

## 📌 Project Overview

EconoCausal is a data science project exploring how causal inference and Double Machine Learning (DML) could help businesses evaluate marketing offers and make better discount-related decisions.

Traditional machine learning often identifies patterns between customer characteristics and purchasing behavior. Causal inference aims to answer a different question: **What effect does an intervention have on an outcome?**

The project investigates the available marketing campaign, coupon, customer demographic, and transaction datasets to determine whether they can support a defensible causal analysis.

> **Current status:** The project is in the exploratory analysis and causal-feasibility assessment stage. A valid treatment variable and causal effect have not yet been established.

## 🎯 Project Objectives

* Inspect and understand the available datasets.
* Assess data quality, missing values, and duplicate records.
* Explore customer, campaign, coupon, and transaction relationships.
* Analyze observed coupon redemption patterns.
* Identify potential treatment, outcome, and covariate variables.
* Investigate whether treatment assignment and campaign exposure can be established.
* Evaluate the assumptions required for Double Machine Learning.
* Maintain reproducible notebooks, daily reports, and analysis outputs.

## 🧠 Key Concepts

### 1. Treatment (T)

The treatment represents the intervention whose effect we want to estimate, such as an assigned discount or marketing offer.

**Current status:** Treatment assignment has not yet been verified in the available data.

Transaction-level discount records cannot automatically be interpreted as assigned treatment for every customer.

### 2. Outcome (Y)

The training dataset contains `redemption_status`, which indicates whether a coupon was redeemed.

This is a candidate outcome variable for studying redemption behavior. However, redemption alone does not establish the causal effect of a discount.

### 3. Covariates (X)

Potential covariates include customer demographic characteristics and campaign-related information.

Before modeling, these variables must be checked for:

* Availability and missingness.
* Relevance to treatment assignment and the outcome.
* Measurement timing.
* Whether they were measured before treatment.
* Potential sources of confounding.

### 4. Double Machine Learning

Double Machine Learning combines machine learning with statistical techniques designed to estimate causal effects while accounting for observed confounders under appropriate assumptions.

Applying DML requires a defensible treatment definition, a suitable outcome, appropriate covariates, and an identification strategy.

The project will proceed to causal modeling only after the available data has been assessed for these requirements.

## 📂 Dataset Overview

The project uses the AmExpert 2019 Marketing Campaign dataset.

The available files include:

| Dataset                         | Description                                            |
| ------------------------------- | ------------------------------------------------------ |
| `train.csv`                     | Training records, including coupon redemption outcomes |
| `test_QyjYwdj.csv`              | Test records                                           |
| `campaign_data.csv`             | Campaign information                                   |
| `customer_demographics.csv`     | Customer demographic information                       |
| `customer_transaction_data.csv` | Historical customer transaction records                |
| `coupon_item_mapping.csv`       | Relationships between coupons and items                |
| `item_data.csv`                 | Item-related information                               |
| `sample_submission_Byiv0dS.csv` | Sample submission format                               |

**Dataset source:** [AmExpert 2019 Marketing Campaign — Kaggle](https://www.kaggle.com/competitions/amexpert-2019/data)

The original data files are stored locally under `data/raw/` and should not be committed to GitHub.

## 📊 Project Progress

| Day | Task                                    | Key Deliverables                                                 | Status    |
| --- | --------------------------------------- | ---------------------------------------------------------------- | --------- |
| 1   | Dataset Inspection                      | Initial dataset summary                                          | Completed |
| 2   | Data Quality Analysis                   | Missing-value and duplicate analysis                             | Completed |
| 3   | Dataset Relationship Validation         | Relationship and training structure summaries                    | Completed |
| 4   | Target and Campaign Analysis            | Redemption and campaign summaries                                | Completed |
| 5   | Customer and Coupon Analysis            | Demographic and coupon-item summaries                            | Completed |
| 6   | Transaction and Discount Analysis       | Transaction, missing-value, duplicate, and correlation summaries | Completed |
| 7   | Dataset Integration                     | Integration and causal-variable summaries                        | Completed |
| 8   | Treatment and Outcome Assessment        | Preliminary causal assessment                                    | Completed |
| 9   | Campaign Exposure Analysis              | Campaign counts and redemption summaries                         | Completed |
| 10  | Customer-Campaign Relationship Analysis | Customer-campaign and coupon relationship summaries              | Completed |
| 11  | Treatment and Outcome Definition        | Preliminary treatment-outcome assessment                         | Completed |

*Progress reflects the work documented in the project workflow. Verify that each notebook and output file is present in the repository.*

## 📁 Repository Structure

```text
EconoCausal/
│
├── README.md
├── .gitignore
├── requirements.txt
│
├── data/
│   ├── raw/                 # Original datasets; excluded from Git
│   └── processed/           # Processed data; excluded from Git
│
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
│   └── 11_treatment_outcome_definition.ipynb
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
    ├── day01_dataset_summary.csv
    ├── day02_missing_values.csv
    ├── day02_duplicate_analysis.csv
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
    ├── day09_campaign_redemption.csv
    ├── day10_customer_campaign_counts.csv
    ├── day10_campaign_coupon_summary.csv
    ├── day10_coupon_campaign_counts.csv
    ├── day10_relationship_validation.csv
    └── day11_treatment_outcome_assessment.csv
```

*This is the intended structure. Some filenames may need to be adjusted to match the files actually present in your repository.*

## 🔬 Work Completed

### Day 1 — Dataset Inspection

Loaded the available datasets and examined their dimensions, columns, and basic structure.

### Day 2 — Data Quality Analysis

Investigated missing values and duplicate records to identify potential data-quality issues.

### Day 3 — Dataset Relationship Validation

Inspected dataset keys and validated relationships between training records and supporting datasets.

### Day 4 — Target and Campaign Analysis

Examined redemption outcomes and explored observed differences across campaigns.

### Day 5 — Customer and Coupon Analysis

Investigated customer demographics, coupon-item mappings, and item-category distributions.

### Day 6 — Transaction and Discount Analysis

Explored transaction records, discount-related variables, missingness, duplicate records, and correlations.

### Day 7 — Dataset Integration

Integrated selected datasets and examined merge relationships, row preservation, and potential causal variables.

### Day 8 — Treatment and Outcome Assessment

Inspected possible treatment and outcome variables and documented uncertainties in the available information.

### Day 9 — Campaign Exposure Analysis

Examined campaign-level records, redemption rates, and the available evidence concerning campaign exposure.

### Day 10 — Customer-Campaign Relationship Analysis

Investigated customer-campaign relationships, coupon distribution, duplicate combinations, and identifier uniqueness.

### Day 11 — Treatment and Outcome Definition

Created a preliminary assessment of the outcome, potential covariates, and identifiers. Documented that a defensible treatment assignment has not yet been verified.

## ⚠️ Causal Inference Considerations

The project distinguishes exploratory findings from causal conclusions.

Before estimating a causal effect, the following questions must be addressed:

1. **Treatment definition:** What intervention was assigned, and how is it recorded?
2. **Exposure:** Can the data establish which customers were eligible for or exposed to the intervention?
3. **Outcome definition:** What result will be measured, and over what period?
4. **Covariate timing:** Which characteristics were measured before treatment?
5. **Confounding:** What factors may influence both treatment assignment and the outcome?
6. **Identification assumptions:** Can the treatment effect be identified from the available observational data?
7. **Data coverage:** Are there enough comparable treated and untreated observations?

Differences in redemption rates do not, by themselves, demonstrate that a discount caused a change in customer behavior.

If the available datasets do not support a defensible causal design, this limitation will be documented rather than hidden behind a predictive model.

## 🛠️ Tools and Technologies

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* JupyterLab
* GitHub
* CSV-based analysis outputs

## ▶️ Getting Started

### 1. Clone or download the repository

Open the repository on GitHub and download the project files to your computer.

### 2. Install dependencies

Open a terminal in the `EconoCausal` directory and run:

```bash
pip install -r requirements.txt
```

### 3. Prepare the data directory

Create the following directory if it does not already exist:

```text
EconoCausal/data/raw/
```

Obtain the dataset from Kaggle and place the required CSV files in that directory.

Do not upload the original datasets to GitHub unless you have confirmed that redistribution is permitted.

### 4. Launch JupyterLab

Run:

```bash
jupyter lab
```

Open the `notebooks/` directory and execute the notebooks in sequence.

**Note:** Notebook paths assume that the notebooks are run from their intended directory and that the datasets are stored under `data/raw/`.

## 📈 Next Steps

The next stage will focus on:

* Investigating potential treatment-assignment variables.
* Examining whether campaign eligibility or exposure can be established.
* Assessing whether the data supports a meaningful treatment comparison.
* Defining an appropriate outcome and pre-treatment covariates.
* Documenting the causal identification strategy and its limitations.
* Deciding whether DML estimation is justified.

Model development and causal effect estimation should follow only after these questions have been addressed.

## 📌 Project Information

* **Project:** EconoCausal — Dynamic Pricing via Double Machine Learning
* **Organization:** Infotact Solutions
* **Domain:** Data Science, Machine Learning, and Causal Inference
* **Current Progress:** Day 11
* **Current Stage:** Exploratory Data Analysis and Causal Feasibility Assessment

---

*This project is being developed as an internship learning exercise. All findings and conclusions will be based on verified data and documented assumptions.*
