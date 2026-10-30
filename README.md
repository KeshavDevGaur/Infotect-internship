# EconoCausal

### Dynamic Pricing and Causal Analysis Using Double Machine Learning

## Project Overview

EconoCausal is a data science research project focused on understanding customer purchasing behaviour, coupon campaigns, and the feasibility of causal analysis using the AmExpert 2019 Marketing Campaign dataset.

The project investigates how promotional campaigns and discounts may influence customer purchasing behaviour. It emphasizes proper treatment definition, outcome construction, identification assumptions, and data quality before applying causal machine learning techniques.

The long-term objective is to evaluate whether Double Machine Learning (DML) can provide reliable estimates of promotional campaign effects.

## Research Objectives

* Understand the structure of the AmExpert 2019 dataset.
* Explore customer, campaign, coupon, product, and transaction information.
* Investigate promotional campaign characteristics.
* Identify possible treatment and outcome variables.
* Examine customer-level purchasing behaviour.
* Evaluate data quality and measurement limitations.
* Study causal identification assumptions.
* Assess the feasibility of Double Machine Learning.
* Develop a reproducible research workflow.

## Dataset

**Dataset:** AmExpert 2019 Marketing Campaign

The dataset contains multiple files related to customers, campaigns, coupons, products, and transactions.

### Dataset Files

| File                            | Description                                                            |
| ------------------------------- | ---------------------------------------------------------------------- |
| `train.csv`                     | Training data containing customer-coupon records and redemption status |
| `test_QyjYwdj.csv`              | Test dataset                                                           |
| `campaign_data.csv`             | Campaign-related information                                           |
| `customer_demographics.csv`     | Customer demographic information                                       |
| `customer_transaction_data.csv` | Customer transaction history                                           |
| `coupon_item_mapping.csv`       | Mapping between coupons and items                                      |
| `item_data.csv`                 | Product and item information                                           |
| `sample_submission_Byiv0dS.csv` | Sample submission format                                               |

**Note:** Raw datasets are stored locally in `data/raw/` and are not included in the GitHub repository.

## Project Structure

```text
EconoCausal/
│
├── data/
│   └── raw/
│       └── (Raw datasets stored locally)
│
├── notebooks/
│   ├── 01_*.ipynb
│   ├── ...
│   ├── 16_dataset_documentation_causal_design.ipynb
│   ├── 17_treatment_definition_identification_strategy.ipynb
│   ├── 18_dataset_documentation_research.ipynb
│   └── README.md
│
├── reports/
│   ├── DAY16_REPORT.md
│   ├── DAY17_REPORT.md
│   ├── DAY18_REPORT.md
│   ├── day16_causal_research_design_assessment.csv
│   ├── day17_treatment_candidate_assessment.csv
│   ├── day17_causal_identification_assessment.csv
│   ├── day17_causal_research_assessment.csv
│   ├── day18_fuel_item_analysis.csv
│   └── README.md
│
└── README.md
```

*The notebook names and report files from earlier days are maintained in their respective folders.*

## Research Progress

### Phase 1: Dataset Exploration and Preparation

**Days 1–15**

Completed the initial project workflow, including dataset exploration, data preparation, descriptive analysis, and preliminary research.

### Phase 2: Causal Research Design

**Day 16 — Dataset Documentation and Causal Design**

* Reviewed dataset structure and available variables.
* Documented the research design.
* Examined potential causal research questions.
* Identified limitations in the available data.

**Day 17 — Treatment Definition and Identification Strategy**

* Evaluated possible treatment variables.
* Examined treatment assignment and exposure limitations.
* Investigated potential outcome variables.
* Assessed causal identification requirements.
* Documented unresolved causal assumptions.

### Phase 3: Dataset Documentation Research

**Day 18 — Transaction Data and Measurement Investigation**

* Investigated original dataset documentation.
* Studied transaction variables and their distributions.
* Examined extreme transaction quantities.
* Investigated Fuel category transaction patterns.
* Analyzed frequently observed Fuel items.
* Compared price-to-quantity ratios.
* Documented limitations in expenditure measurement.

**Important finding:** Six frequently observed Fuel items showed relatively consistent price-to-quantity ratios, with a mean of approximately 0.086807.

## Causal Research Considerations

The project follows an important principle:

**Prediction does not automatically imply causation.**

Before estimating campaign effects, the research must establish:

1. A clearly defined treatment or intervention.
2. A defensible treatment assignment mechanism.
3. A properly measured outcome variable.
4. Relevant pre-treatment confounders.
5. Appropriate identification assumptions.
6. Sufficient data quality and overlap.

The `redemption_status` variable is a potential outcome candidate, but coupon redemption alone does not establish whether a customer was exposed to or assigned a campaign.

Campaign types X and Y are anonymized categories and should not automatically be interpreted as treatment and control groups.

Double Machine Learning is an estimation method; it does not independently solve problems of treatment assignment or causal identification.

## Technology Stack

* Python
* Jupyter Notebook / JupyterLab
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* Git and GitHub

## Current Limitations

* Actual campaign exposure is not yet established.
* Treatment assignment mechanism remains unresolved.
* Campaign type labels are anonymized.
* Customer demographic information is not available for every training record.
* Transaction quantity units require further documentation.
* A defensible customer expenditure outcome is still under investigation.
* Causal identification assumptions require additional verification.

## Future Work

* Investigate transaction variable definitions and measurement units.
* Develop a defensible customer-level outcome.
* Further investigate campaign exposure and treatment assignment.
* Evaluate confounding and overlap.
* Finalize the causal research design.
* Assess DML model feasibility.
* Conduct estimation only after the identification strategy is justified.
* Evaluate robustness and interpretability.

## Project Status

**Completed:** Day 18
**Current Focus:** Dataset documentation, treatment definition, and causal identification research.

## Author

Developed as part of a Data Science internship project.

**Project:** EconoCausal — Dynamic Pricing via Double Machine Learning
