# EconoCausal — Dynamic Pricing via Double Machine Learning

## Project Overview

EconoCausal is a data science and causal inference project exploring customer behavior, marketing campaigns, coupon redemption, and the feasibility of estimating treatment effects using Double Machine Learning (DML).

The project emphasizes data quality, relationship validation, treatment and outcome definition, and the assumptions required for defensible causal inference.

## Objectives

* Explore and validate the available datasets.
* Analyze customer, campaign, coupon, and transaction relationships.
* Investigate coupon redemption and customer behavior.
* Identify candidate treatment and outcome variables.
* Assess treatment assignment and customer-level campaign exposure.
* Evaluate whether the available data supports a defensible causal identification strategy.

## Dataset

**Dataset:** AmExpert 2019 Marketing Campaign

| Dataset                         | Purpose                                 |
| ------------------------------- | --------------------------------------- |
| `train.csv`                     | Training records and redemption outcome |
| `test_QyjYwdj.csv`              | Test dataset                            |
| `campaign_data.csv`             | Campaign metadata                       |
| `customer_demographics.csv`     | Customer demographic information        |
| `customer_transaction_data.csv` | Customer transaction history            |
| `coupon_item_mapping.csv`       | Coupon-to-item mapping                  |
| `item_data.csv`                 | Item metadata                           |
| `sample_submission_Byiv0dS.csv` | Sample submission format                |

Raw datasets are stored locally and excluded from GitHub.

## Project Structure

```text
EconoCausal/
├── .gitignore
├── requirements.txt
├── README.md
├── data/
│   ├── raw/
│   └── processed/
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
│   ├── 12_treatment_assignment_analysis.ipynb
│   ├── 13_customer_exposure_analysis.ipynb
│   └── 14_causal_identification_feasibility.ipynb
└── reports/
    ├── README.md
    ├── DAY1_REPORT.md through DAY14_REPORT.md
    └── day14_causal_identification_assessment.csv
```

*This is the intended structure. Verify that each listed file exists before treating the listing as a complete inventory.*

## Progress Tracker

| Day | Work Completed                                      |
| --- | --------------------------------------------------- |
| 1   | Dataset inspection and initial summary              |
| 2   | Data quality and duplicate analysis                 |
| 3   | Dataset relationship validation                     |
| 4   | Target and campaign redemption analysis             |
| 5   | Customer demographics and coupon analysis           |
| 6   | Transaction and discount analysis                   |
| 7   | Dataset integration and causal variable exploration |
| 8   | Preliminary causal feasibility assessment           |
| 9   | Campaign exposure investigation                     |
| 10  | Customer-campaign relationship analysis             |
| 11  | Treatment and outcome assessment                    |
| 12  | Treatment assignment investigation                  |
| 13  | Customer-level relationship and exposure assessment |
| 14  | Causal identification feasibility assessment        |

## Day 14 Highlights

* Inspected training, campaign, customer demographic, and transaction datasets.
* Reviewed candidate treatment and outcome variables.
* Investigated potential confounders and variable timing.
* Examined available campaign and transaction date information.
* Documented unresolved questions about treatment assignment and causal identification.
* Generated `day14_causal_identification_assessment.csv`.

## Methodology and Tools

* **Language:** Python
* **Data analysis:** Pandas, NumPy
* **Environment:** JupyterLab
* **Version control:** GitHub
* **Planned causal method:** Double Machine Learning

## Causal Inference Considerations

The `redemption_status` variable is a candidate outcome, but its suitability depends on the causal question.

A verified treatment variable and assignment mechanism have not yet been established. Campaign identifiers, campaign characteristics, coupon redemption, and transaction discounts do not independently establish treatment assignment or actual exposure.

Before estimating causal effects, the project must establish:

1. A clearly defined causal question.
2. A valid treatment variable and its assignment mechanism.
3. A suitable outcome and measurement period.
4. Appropriate pre-treatment covariates.
5. A defensible identification strategy and its assumptions.

Potential covariates must be checked for timing and relevance. Post-treatment variables should not be treated as baseline confounders without careful justification.

## Current Status

**Completed through Day 14:** Initial data exploration, data quality checks, relationship validation, descriptive analysis, treatment and outcome investigation, and preliminary causal feasibility assessment.

**Next priority:** Investigate the evidence needed to establish treatment assignment and determine whether the available data supports a credible causal identification strategy.

## Data Handling

Raw datasets are excluded from version control. Follow the dataset's applicable license and terms when using or sharing data.
