# EconoCausal — Dynamic Pricing via Double Machine Learning

## Project Overview

EconoCausal is a data science and causal inference project exploring marketing campaign data, customer behavior, coupon redemption, and the requirements for estimating treatment effects using Double Machine Learning (DML).

The project emphasizes identifying defensible treatment and outcome variables, validating data relationships, and distinguishing descriptive associations from causal evidence.

## Objectives

* Explore and validate the available datasets.
* Analyze customer, campaign, coupon, and transaction relationships.
* Investigate coupon redemption patterns.
* Examine potential treatment and outcome definitions.
* Assess whether treatment assignment and customer-level exposure can be verified.
* Establish the assumptions needed for a defensible causal analysis.

## Dataset

**Dataset:** AmExpert 2019 Marketing Campaign

The project uses the following datasets:

| Dataset                         | Purpose                                        |
| ------------------------------- | ---------------------------------------------- |
| `train.csv`                     | Training records and coupon redemption outcome |
| `test_QyjYwdj.csv`              | Test dataset                                   |
| `campaign_data.csv`             | Campaign metadata                              |
| `customer_demographics.csv`     | Customer demographic information               |
| `customer_transaction_data.csv` | Customer transaction history                   |
| `coupon_item_mapping.csv`       | Coupon-to-item mapping                         |
| `item_data.csv`                 | Item metadata                                  |
| `sample_submission_Byiv0dS.csv` | Sample submission format                       |

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
│   └── 13_customer_exposure_analysis.ipynb
└── reports/
    ├── README.md
    ├── DAY1_REPORT.md through DAY13_REPORT.md
    └── day13_customer_exposure_assessment.csv
```

*Note: This structure describes the intended organization. Ensure each listed file exists and has been uploaded before treating the listing as a complete inventory.*

## Progress Tracker

| Day    | Work Completed                                       |
| ------ | ---------------------------------------------------- |
| Day 1  | Dataset inspection and initial summary               |
| Day 2  | Data quality and duplicate analysis                  |
| Day 3  | Dataset relationship validation                      |
| Day 4  | Target and campaign redemption analysis              |
| Day 5  | Customer demographics and coupon analysis            |
| Day 6  | Transaction and discount analysis                    |
| Day 7  | Dataset integration and causal variable exploration  |
| Day 8  | Preliminary causal feasibility assessment            |
| Day 9  | Campaign exposure investigation                      |
| Day 10 | Customer-campaign relationship analysis              |
| Day 11 | Preliminary treatment and outcome definition         |
| Day 12 | Treatment assignment investigation                   |
| Day 13 | Customer-level relationships and exposure assessment |

## Day 13 Highlights

* Examined customer-level campaign and coupon relationships.
* Validated customer, campaign, and coupon identifiers.
* Investigated repeated customer–campaign–coupon combinations.
* Created `day13_customer_exposure_assessment.csv`.
* Documented limitations in establishing actual customer-level campaign exposure.

## Methodology and Tools

* **Language:** Python
* **Data analysis:** Pandas, NumPy
* **Environment:** JupyterLab
* **Version control:** GitHub
* **Planned causal method:** Double Machine Learning

## Causal Inference Considerations

Coupon redemption is an observed outcome, not proof of treatment assignment. Similarly, identifier matches and campaign associations do not independently establish that a customer received or was exposed to a particular treatment.

Before estimating causal effects, the project must establish:

1. A clearly defined treatment variable.
2. A clearly defined outcome.
3. A defensible treatment-assignment or identification strategy.
4. Appropriate pre-treatment confounders.
5. Assumptions required for the proposed causal estimator.

The availability of suitable treatment and exposure data remains an open question.

## Current Status

**Completed through Day 13:** Initial data exploration, relationship validation, descriptive analysis, and preliminary causal feasibility assessments.

**Next priority:** Resolve treatment assignment and exposure, then determine whether the available data supports a defensible causal identification strategy.

## Data Handling

Raw datasets are excluded from version control. Follow the dataset's applicable license and terms when using or sharing data.
