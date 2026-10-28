# EconoCausal — Dynamic Pricing via Double Machine Learning

## Project Overview

EconoCausal is a data science and causal inference project exploring marketing campaigns, customer behavior, coupon redemption, and the feasibility of estimating causal effects using Double Machine Learning (DML).

The project focuses on data validation, campaign analysis, treatment definition, treatment-assignment investigation, and the assumptions required for defensible causal inference.

## Objectives

* Explore and validate the available datasets.
* Analyze customer, campaign, coupon, and transaction relationships.
* Investigate coupon redemption patterns.
* Examine candidate treatment and outcome variables.
* Assess customer eligibility, treatment assignment, and campaign exposure.
* Investigate dataset documentation and campaign-generation information.
* Evaluate whether the available evidence supports a defensible causal research design.

## Dataset

**Dataset:** AmExpert 2019 Marketing Campaign

| Dataset                         | Purpose                                          |
| ------------------------------- | ------------------------------------------------ |
| `train.csv`                     | Training records and observed redemption outcome |
| `test_QyjYwdj.csv`              | Test dataset                                     |
| `campaign_data.csv`             | Campaign metadata                                |
| `customer_demographics.csv`     | Customer demographic information                 |
| `customer_transaction_data.csv` | Customer transaction history                     |
| `coupon_item_mapping.csv`       | Coupon-to-item mapping                           |
| `item_data.csv`                 | Item metadata                                    |
| `sample_submission_Byiv0dS.csv` | Sample submission format                         |

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
│   ├── 15_treatment_assignment_evidence.ipynb
│   └── 16_dataset_documentation_causal_design.ipynb
└── reports/
    ├── README.md
    ├── DAY1_REPORT.md through DAY16_REPORT.md
    └── day16_causal_research_design_assessment.csv
```

*This is the intended structure. Verify that each listed file exists before treating this as a complete inventory.*

## Progress Tracker

| Day | Work Completed                                              |
| --- | ----------------------------------------------------------- |
| 1   | Initial dataset inspection                                  |
| 2   | Data quality and duplicate analysis                         |
| 3   | Dataset relationship validation                             |
| 4   | Target and campaign analysis                                |
| 5   | Customer demographics and coupon analysis                   |
| 6   | Transaction and discount analysis                           |
| 7   | Dataset integration and causal variable exploration         |
| 8   | Preliminary causal feasibility assessment                   |
| 9   | Campaign exposure investigation                             |
| 10  | Customer-campaign relationship analysis                     |
| 11  | Treatment and outcome assessment                            |
| 12  | Treatment-assignment investigation                          |
| 13  | Customer-level relationship and exposure assessment         |
| 14  | Causal identification feasibility assessment                |
| 15  | Treatment-assignment evidence investigation                 |
| 16  | Dataset documentation and causal research design assessment |

## Day 16 Highlights

* Inspected campaign metadata and training dataset structure.
* Examined campaign types X and Y.
* Compared observed redemption patterns across campaign types.
* Documented questions about campaign meaning, customer eligibility, treatment assignment, and actual exposure.
* Created `day16_causal_research_design_assessment.csv`.

## Tools and Methodology

* **Language:** Python
* **Libraries:** Pandas, NumPy
* **Environment:** JupyterLab
* **Version control:** GitHub
* **Planned causal method:** Double Machine Learning

## Causal Inference Considerations

The `redemption_status` variable is a candidate observed outcome. It does not independently establish treatment assignment.

Campaign identifiers and campaign types provide descriptive information. They do not independently prove which customers received an intervention or whether that intervention caused observed outcomes.

Before estimating causal effects, the project must establish:

1. A precise causal question.
2. A clearly defined treatment and outcome.
3. Evidence supporting treatment assignment or a defensible identification strategy.
4. Appropriate pre-treatment covariates.
5. Justified assumptions for causal estimation.

Observed differences between campaign types should not be presented as causal effects without supporting evidence.

## Current Status

**Completed through Day 16:** Data exploration, data quality checks, relationship validation, descriptive campaign analysis, treatment and outcome investigation, and preliminary causal research-design assessments.

**Next priority:** Verify the documented meaning of campaign types, investigate the available evidence of customer assignment and exposure, and determine whether the data supports a credible causal identification strategy.

## Data Handling

Raw datasets are excluded from version control. Follow the dataset's applicable license and terms when using or sharing data.
