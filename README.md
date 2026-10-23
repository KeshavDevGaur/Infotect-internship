# EconoCausal — Dynamic Pricing via Double Machine Learning

**Internship Project | Infotact Solutions | Data Science & Causal Inference**

## 📌 Project Overview

EconoCausal explores how causal inference and Double Machine Learning (DML) could help businesses evaluate marketing offers and make better discount-related decisions.

Traditional machine learning identifies patterns between customer characteristics and purchasing behavior. Causal inference aims to answer a different question: **What effect does an intervention have on an outcome?**

This project investigates marketing campaign, coupon, customer demographic, and transaction datasets to determine whether they can support a defensible causal analysis.

> **Current status:** Exploratory data analysis and causal-feasibility assessment. A verified treatment assignment and causal effect have not yet been established.

## 🎯 Project Objectives

* Inspect and understand the available datasets.
* Assess data quality, missing values, and duplicate records.
* Explore customer, campaign, coupon, and transaction relationships.
* Analyze observed coupon redemption patterns.
* Identify potential treatment, outcome, and covariate variables.
* Investigate whether treatment assignment and campaign exposure can be established.
* Evaluate assumptions required for Double Machine Learning.
* Maintain reproducible notebooks, reports, and analysis outputs.

## 🧠 Key Concepts

### 1. Treatment (T)

Treatment represents the intervention whose effect we want to estimate, such as an assigned discount or marketing offer.

**Status:** Treatment assignment has not yet been verified in the available data.

Transaction-level discount records cannot automatically be interpreted as assigned treatment for every customer.

### 2. Outcome (Y)

The training dataset contains `redemption_status`, indicating whether a coupon was redeemed.

This is a candidate outcome for studying redemption behavior. It does not independently establish the causal effect of a discount.

### 3. Covariates (X)

Potential covariates include customer demographics and campaign characteristics. Their timing, relevance, missingness, and relationship to treatment assignment must be assessed before modeling.

### 4. Double Machine Learning

Double Machine Learning combines machine learning with statistical techniques for estimating causal effects while accounting for observed confounders under appropriate assumptions.

A defensible DML analysis requires a clearly defined treatment, a suitable outcome, appropriate covariates, and a credible identification strategy.

## 📂 Dataset Overview

The project uses the AmExpert 2019 Marketing Campaign dataset.

| Dataset                         | Description                                            |
| ------------------------------- | ------------------------------------------------------ |
| `train.csv`                     | Training records, including coupon redemption outcomes |
| `test_QyjYwdj.csv`              | Test records                                           |
| `campaign_data.csv`             | Campaign information                                   |
| `customer_demographics.csv`     | Customer demographic information                       |
| `customer_transaction_data.csv` | Historical transaction records                         |
| `coupon_item_mapping.csv`       | Relationships between coupons and items                |
| `item_data.csv`                 | Item-related information                               |
| `sample_submission_Byiv0dS.csv` | Sample submission format                               |

**Dataset source:** [AmExpert 2019 Marketing Campaign — Kaggle](https://www.kaggle.com/competitions/amexpert-2019/data)

The original datasets are stored locally in `data/raw/` and should not be committed to GitHub.

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
| 12  | Treatment Assignment Analysis           | Campaign metadata inspection and treatment-assignment assessment | Completed |

*Progress reflects the work documented in the project workflow. Verify that the notebooks and outputs are present in the repository.*

## 📁 Repository Structure

```text
EconoCausal/
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
    └── [CSV analysis outputs]
```

*This is the intended structure. Adjust filenames to match the files actually present in the repository.*

## 🔬 Work Completed

### Day 1 — Dataset Inspection

Loaded the available datasets and examined their dimensions, columns, and basic structure.

### Day 2 — Data Quality Analysis

Investigated missing values and duplicate records.

### Day 3 — Dataset Relationship Validation

Inspected dataset keys and validated relationships between training records and supporting datasets.

### Day 4 — Target and Campaign Analysis

Examined redemption outcomes and explored observed differences across campaigns.

### Day 5 — Customer and Coupon Analysis

Investigated customer demographics, coupon-item mappings, and item-category distributions.

### Day 6 — Transaction and Discount Analysis

Explored transaction records, discount-related variables, missingness, duplicates, and correlations.

### Day 7 — Dataset Integration

Integrated selected datasets and examined merge relationships, row preservation, and potential causal variables.

### Day 8 — Treatment and Outcome Assessment

Inspected potential treatment and outcome variables and documented uncertainties in the available information.

### Day 9 — Campaign Exposure Analysis

Examined campaign-level records, redemption rates, and evidence concerning campaign exposure.

### Day 10 — Customer-Campaign Relationship Analysis

Investigated customer-campaign relationships, coupon distribution, duplicate combinations, and identifier uniqueness.

### Day 11 — Treatment and Outcome Definition

Created a preliminary assessment of the outcome, potential covariates, and identifiers. Documented that a defensible treatment assignment had not been verified.

### Day 12 — Treatment Assignment Analysis

Inspected campaign metadata, examined campaign types and dates, compared observed redemption patterns, and documented the limitations of the available evidence for identifying treatment assignment.

## ⚠️ Causal Inference Considerations

Before estimating a causal effect, the project must address:

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

### 1. Obtain the project

Download the repository from GitHub and open the `EconoCausal` directory.

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Prepare the datasets

Place the required CSV files in `data/raw/`.

Obtain the dataset from Kaggle and confirm that redistribution is permitted before sharing any raw data.

### 4. Launch JupyterLab

```bash
jupyter lab
```

Open the `notebooks/` directory and execute the notebooks in sequence.

Notebook paths assume that the datasets are stored under `data/raw/` and that notebooks are run from their intended directory.

## 📈 Next Steps

* Investigate the meaning of campaign types.
* Determine whether customer-level treatment assignment can be established reliably.
* Examine the available customer-campaign and coupon relationships.
* Identify suitable pre-treatment covariates.
* Document the causal identification strategy and its limitations.
* Decide whether DML estimation is justified.

## 📌 Project Information

* **Project:** EconoCausal — Dynamic Pricing via Double Machine Learning
* **Organization:** Infotact Solutions
* **Domain:** Data Science, Machine Learning, and Causal Inference
* **Current Progress:** Day 12
* **Current Stage:** Exploratory Data Analysis and Causal Feasibility Assessment

---

*All findings and conclusions should be based on verified data and documented assumptions.*
