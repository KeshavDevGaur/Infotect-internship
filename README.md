# EconoCausal — Dynamic Pricing via Double Machine Learning

## Project Overview

**EconoCausal** is a data science research project focused on investigating customer coupon redemption, campaign characteristics, and the feasibility of estimating causal effects using Double Machine Learning (DML).

The project uses the AmExpert 2019 Marketing Campaign dataset to explore customer behavior, campaign information, coupon-item relationships, transaction data, and potential causal research designs.

The primary objective is to establish a defensible treatment definition and causal identification strategy before estimating any treatment effect.

> **Important:** The current analysis is exploratory. A causal effect has not yet been established, and the available data have not yet been shown to support a valid DML estimation strategy.

---

## Project Objectives

* Inspect and understand the available datasets.
* Assess data quality, missing values, and duplicate records.
* Validate relationships between datasets.
* Analyze coupon redemption patterns.
* Explore customer demographics and campaign characteristics.
* Investigate transaction and discount information.
* Evaluate potential treatment and outcome definitions.
* Investigate campaign assignment and customer exposure.
* Assess potential confounding variables.
* Evaluate possible causal identification strategies.
* Document the assumptions and evidence required for Double Machine Learning.

---

## Technology Stack

| Technology              | Purpose                                                                 |
| ----------------------- | ----------------------------------------------------------------------- |
| Python                  | Data analysis and research                                              |
| Pandas                  | Data manipulation and integration                                       |
| NumPy                   | Numerical analysis                                                      |
| Matplotlib              | Data visualization                                                      |
| Seaborn                 | Statistical visualization                                               |
| JupyterLab              | Interactive notebooks                                                   |
| GitHub                  | Version control and project documentation                               |
| Scikit-learn            | Potential machine learning models                                       |
| Double Machine Learning | Planned causal estimation method, subject to identification feasibility |

---

## Dataset Overview

The project uses the AmExpert 2019 Marketing Campaign dataset.

### Main datasets

| Dataset                         | Description                                                                        |
| ------------------------------- | ---------------------------------------------------------------------------------- |
| `train.csv`                     | Training records containing customer, campaign, coupon, and redemption information |
| `test_QyjYwdj.csv`              | Test records                                                                       |
| `campaign_data.csv`             | Campaign metadata, including campaign identifiers, types, and dates                |
| `customer_demographics.csv`     | Customer demographic information                                                   |
| `customer_transaction_data.csv` | Customer transaction records                                                       |
| `coupon_item_mapping.csv`       | Relationships between coupons and items                                            |
| `item_data.csv`                 | Item information                                                                   |
| `sample_submission_Byiv0dS.csv` | Sample submission format                                                           |

### Data management

Raw datasets are stored locally in `data/raw/` and are excluded from Git tracking.

Raw data should not be uploaded to GitHub as part of this project.

---

## Repository Structure

```text
EconoCausal/
│
├── README.md
├── .gitignore
├── requirements.txt
│
├── data/
│   ├── raw/
│   └── processed/
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
│   ├── 12_treatment_assignment_analysis.ipynb
│   ├── 13_customer_exposure_analysis.ipynb
│   ├── 14_causal_identification_feasibility.ipynb
│   ├── 15_treatment_assignment_evidence.ipynb
│   └── 16_dataset_documentation_causal_design.ipynb
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
    ├── DAY13_REPORT.md
    ├── DAY14_REPORT.md
    ├── DAY15_REPORT.md
    ├── DAY16_REPORT.md
    ├── DAY17_REPORT.md
    └── [Assessment CSV files]
```

**Note:** The structure above documents the intended organization. Ensure that each listed notebook and report actually exists before considering the repository structure complete.

---

## Daily Progress

### Day 1 — Dataset Inspection

* Loaded and inspected the available datasets.
* Examined dataset dimensions, columns, and basic structure.
* Created an initial dataset summary.

### Day 2 — Data Quality Analysis

* Investigated missing values.
* Examined duplicate records.
* Documented data quality findings.

### Day 3 — Dataset Relationships

* Investigated relationships between dataset identifiers.
* Validated key relationships between campaign, customer, and coupon data.
* Documented relationship checks.

### Day 4 — Redemption Analysis

* Examined the redemption target distribution.
* Investigated campaign-level redemption patterns.
* Compared descriptive results across campaign types.

### Day 5 — Customer and Coupon Analysis

* Explored customer demographic characteristics.
* Examined coupon-item relationships.
* Investigated item category distributions and customer-level patterns.

### Day 6 — Transaction and Discount Analysis

* Inspected transaction data.
* Investigated missing values and duplicate records.
* Explored available discount-related variables.

### Day 7 — Dataset Integration

* Integrated relevant datasets for exploratory analysis.
* Reviewed the availability of potential causal variables.
* Documented integration findings and limitations.

### Day 8 — Initial Causal Assessment

* Reviewed potential causal variables.
* Documented preliminary feasibility considerations.
* Identified unresolved treatment and outcome questions.

### Day 9 — Campaign Exposure Analysis

* Investigated campaign counts and redemption patterns.
* Examined available campaign information.
* Distinguished descriptive campaign comparisons from causal conclusions.

### Day 10 — Customer-Campaign Relationships

* Investigated customer and campaign relationships.
* Examined campaign-coupon associations.
* Validated available identifier relationships.

### Day 11 — Treatment and Outcome Definition

* Reviewed candidate treatment and outcome variables.
* Documented uncertainties in their definitions.
* Identified evidence required for a defensible causal analysis.

### Day 12 — Treatment Assignment Analysis

* Investigated available evidence about treatment assignment.
* Documented unresolved questions concerning how customers were assigned to campaigns.

### Day 13 — Customer Exposure Analysis

* Examined available information relevant to customer exposure.
* Documented limitations in establishing whether customers actually received or encountered an intervention.

### Day 14 — Causal Identification Feasibility

* Assessed the feasibility of causal identification.
* Documented assumptions and evidence required for causal estimation.

### Day 15 — Treatment Assignment Evidence

* Consolidated the available evidence concerning treatment assignment.
* Documented remaining gaps and verification requirements.

### Day 16 — Dataset Documentation and Causal Design

* Reviewed campaign metadata and campaign types.
* Examined campaign and redemption patterns.
* Documented questions concerning campaign interpretation, customer eligibility, assignment, and exposure.
* Created a causal research design assessment.
* Identified additional documentation required before defining a valid intervention.

### Day 17 — Treatment Definition and Causal Identification Strategy

* Inspected candidate treatment and outcome variables.
* Evaluated campaign characteristics and customer covariates.
* Investigated potential confounding variables.
* Assessed randomized experiments, observational adjustment, difference-in-differences, and instrumental variables as possible identification strategies.
* Created the following assessment files:

  * `day17_treatment_candidate_assessment.csv`
  * `day17_causal_identification_assessment.csv`
  * `day17_causal_research_assessment.csv`
* Created `DAY17_REPORT.md`.

**Day 17 conclusion:** The available evidence does not yet establish a defensible treatment definition or causal identification strategy. Further investigation is required before a causal effect can be estimated.

---

## Causal Research Considerations

### 1. Treatment Definition

A valid treatment variable must represent a clearly defined intervention.

The presence of `campaign_id` and `campaign_type` does not, by itself, establish which intervention a customer received.

The meanings of campaign types X and Y and their assignment mechanisms must be verified using appropriate documentation.

### 2. Outcome Definition

The `redemption_status` variable is a candidate outcome for studying coupon redemption.

Its precise meaning and relationship to the intended business intervention must be verified. Coupon redemption alone does not establish actual campaign exposure.

### 3. Potential Confounding Variables

Customer demographics and campaign characteristics may be useful covariates. Their suitability depends on their timing, relevance, and relationships with treatment assignment and the outcome.

Variables measured after treatment may be inappropriate for adjustment in some causal designs.

### 4. Causal Identification

A credible causal analysis requires a justified identification strategy.

Potential approaches include:

* Randomized experiments, when treatment randomization is documented.
* Observational adjustment, when the relevant assumptions and covariates can be justified.
* Difference-in-differences, when suitable comparison groups, time periods, and identifying assumptions are available.
* Instrumental variables, when a valid instrument and the required assumptions can be defended.

These methods cannot be selected solely because the dataset contains customer, campaign, or transaction variables.

### 5. Double Machine Learning

Double Machine Learning can help estimate causal effects under an appropriate identification strategy and its required assumptions.

It does not automatically eliminate unmeasured confounding, establish treatment assignment, or turn descriptive associations into causal effects.

**DML estimation remains conditional on establishing a valid treatment, an appropriate outcome, and a defensible identification strategy.**

---

## Current Project Status

| Area                                | Status                                |
| ----------------------------------- | ------------------------------------- |
| Dataset inspection                  | Completed                             |
| Data quality investigation          | Completed                             |
| Dataset relationship analysis       | Completed                             |
| Redemption and customer exploration | Completed                             |
| Dataset integration investigation   | Completed                             |
| Treatment and outcome exploration   | Completed                             |
| Treatment assignment investigation  | In progress                           |
| Customer exposure verification      | In progress                           |
| Causal identification assessment    | Exploratory                           |
| DML implementation                  | Pending causal feasibility assessment |

These statuses reflect the documented project work. They should be updated if additional evidence changes the conclusions.

---

## Next Steps

1. Verify the original dataset documentation and campaign assignment process.
2. Establish what campaign types X and Y represent.
3. Determine whether treatment assignment or actual customer exposure data are available.
4. Confirm the outcome definition and measurement timing.
5. Identify appropriate pre-treatment covariates and assess potential confounding.
6. Select an identification strategy only if its assumptions are defensible.
7. Determine whether the available data support DML estimation.
8. If causal identification is not possible, document the limitation and consider a clearly labeled predictive or descriptive analysis instead.

---

## Reproducibility and Data Handling

* Keep raw datasets in `data/raw/`.
* Do not upload raw dataset CSV files to GitHub.
* Exclude raw and processed data, virtual environments, secrets, and temporary files from version control as appropriate.
* Store notebooks, reports, and selected derived assessment files in their intended folders.
* Record assumptions and limitations alongside results.
* Verify that all documented files exist in the repository.

---

## Final Note

EconoCausal prioritizes defensible causal reasoning over producing a numerical treatment effect prematurely.

The immediate objective is to establish what intervention is being studied, how treatment is assigned, what outcome is measured, and which assumptions can be justified. Only then should Double Machine Learning be considered for causal estimation.
