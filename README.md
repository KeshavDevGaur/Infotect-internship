# EconoCausal — Dynamic Pricing via Double Machine Learning

## Project Overview

EconoCausal is a data science and causal inference project exploring marketing campaigns, customer behavior, coupon redemption, and the feasibility of estimating causal effects using Double Machine Learning (DML).

The project emphasizes data validation, treatment and outcome definition, treatment-assignment investigation, and the assumptions required for defensible causal inference.

## Objectives

* Explore and validate the available datasets.
* Analyze customer, campaign, coupon, and transaction relationships.
* Investigate coupon redemption patterns.
* Examine potential treatment and outcome variables.
* Assess customer eligibility, treatment assignment, and campaign exposure.
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
│   ├── 14_causal_identification_feasibility.ipynb
│   └── 15_treatment_assignment_evidence.ipynb
└── reports/
    ├── README.md
    ├── DAY1_REPORT.md through DAY15_REPORT.md
    └── day15_treatment_assignment_evidence.csv
```

*This is the intended structure. Verify that each listed file exists before treating this listing as a complete inventory.*

## Progress Tracker

| Day | Work Completed                                      |
| --- | --------------------------------------------------- |
| 1   | Initial dataset inspection                          |
| 2   | Data quality and duplicate analysis                 |
| 3   | Dataset relationship validation                     |
| 4   | Target and campaign analysis                        |
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
| 15  | Treatment-assignment evidence investigation         |

## Day 15 Highlights

* Inspected training, campaign, and customer demographic datasets.
* Examined columns potentially related to treatment, assignment, eligibility, delivery, and exposure.
* Investigated campaign types and campaign-level record counts.
* Compared observed redemption rates descriptively across campaign types.
* Documented unresolved questions about treatment definition and customer exposure.
* Generated `day15_treatment_assignment_evidence.csv`.

## Tools and Methodology

* **Language:** Python
* **Libraries:** Pandas, NumPy
* **Environment:** JupyterLab
* **Version control:** GitHub
* **Planned causal method:** Double Machine Learning

## Causal Inference Considerations

The `redemption_status` variable is a candidate observed outcome. However, coupon redemption does not establish treatment assignment.

Campaign identifiers and campaign types describe campaign relationships and characteristics but do not independently establish which customers received an intervention.

Before estimating causal effects, the project must establish:

1. A precise causal question.
2. A clearly defined treatment and outcome.
3. Evidence of customer eligibility, treatment assignment, or actual exposure.
4. Appropriate pre-treatment covariates.
5. A defensible causal identification strategy and its assumptions.

Descriptive differences in redemption rates must not be presented as causal effects without appropriate identification.

## Current Status

**Completed through Day 15:** Data exploration, relationship validation, descriptive analysis, treatment and outcome investigation, and preliminary causal feasibility assessments.

**Next priority:** Investigate available dataset documentation and campaign-generation information to determine whether a credible treatment contrast and causal identification strategy can be established.

## Data Handling

Raw datasets are excluded from version control. Follow the dataset's applicable license and terms when using or sharing data.
