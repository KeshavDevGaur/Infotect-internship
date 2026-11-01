# EconoCausal

### Dynamic Pricing and Causal Analysis Using Double Machine Learning

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellow)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange)
![Project Status](https://img.shields.io/badge/Progress-Day%2020-success)

## 1. Project Overview

EconoCausal is a data science research project focused on understanding customer purchasing behaviour, promotional campaigns, discounts, and the feasibility of causal analysis using the AmExpert 2019 Marketing Campaign dataset.

The project investigates whether promotional campaigns and coupon-based discounts influence customer purchasing behaviour and expenditure.

The long-term objective is to evaluate whether Double Machine Learning (DML) can provide reliable estimates of promotional campaign effects.

Unlike conventional predictive modelling, this project focuses on understanding causal relationships rather than simply identifying correlations.

## 2. Main Research Goal

The primary research question is:

**Do promotional campaigns and coupon discounts actually cause changes in customer purchasing behaviour and expenditure?**

The project aims to investigate:

* Whether promotional offers increase customer spending.
* Whether coupon campaigns influence purchasing behaviour.
* Which customers respond to promotional interventions.
* Whether discounts generate additional purchasing activity.
* How businesses can improve promotional strategies using causal insights.

## 3. Research Objectives

* Understand customer purchasing behaviour.
* Explore promotional campaign characteristics.
* Analyze coupon and transaction information.
* Investigate customer-level spending patterns.
* Identify potential treatment and outcome variables.
* Evaluate treatment assignment and campaign exposure.
* Investigate confounding and identification assumptions.
* Assess the feasibility of Double Machine Learning.
* Develop a reproducible causal research workflow.

## 4. Dataset Information

**Dataset:** AmExpert 2019 Marketing Campaign

The dataset contains customer, campaign, coupon, product, and transaction information.

### Dataset Files

| File                            | Description                                                            |
| ------------------------------- | ---------------------------------------------------------------------- |
| `train.csv`                     | Training data containing customer-coupon records and redemption status |
| `test_QyjYwdj.csv`              | Test dataset                                                           |
| `campaign_data.csv`             | Campaign-related information                                           |
| `customer_demographics.csv`     | Customer demographic information                                       |
| `customer_transaction_data.csv` | Customer transaction history                                           |
| `coupon_item_mapping.csv`       | Coupon-to-item mapping                                                 |
| `item_data.csv`                 | Product and item information                                           |
| `sample_submission_Byiv0dS.csv` | Sample submission format                                               |

**Note:** Raw datasets are stored locally in `data/raw/` and are not uploaded to GitHub.

## 5. Project Structure

```text
EconoCausal/
│
├── data/
│   └── raw/
│       └── Raw datasets (not uploaded)
│
├── notebooks/
│   ├── Day 01–15 notebooks
│   ├── 16_dataset_documentation_causal_design.ipynb
│   ├── 17_treatment_definition_identification_strategy.ipynb
│   ├── 18_dataset_documentation_research.ipynb
│   ├── 19_transaction_outcome_validation.ipynb
│   ├── 20_transaction_measurement_outcome_feasibility.ipynb
│   └── README.md
│
├── reports/
│   ├── DAY16_REPORT.md
│   ├── DAY17_REPORT.md
│   ├── DAY18_REPORT.md
│   ├── DAY19_REPORT.md
│   ├── DAY20_REPORT.md
│   ├── day16_causal_research_design_assessment.csv
│   ├── day17_treatment_candidate_assessment.csv
│   ├── day17_causal_identification_assessment.csv
│   ├── day17_causal_research_assessment.csv
│   ├── day18_fuel_item_analysis.csv
│   ├── day19_customer_spending_analysis.csv
│   ├── day20_outcome_feasibility_assessment.csv
│   └── README.md
│
└── README.md
```

## 6. Research Progress

### Phase 1 — Initial Data Analysis (Days 1–15)

Completed the initial project workflow, including:

* Dataset exploration.
* Data inspection and preparation.
* Customer and campaign investigation.
* Preliminary descriptive analysis.
* Initial research documentation.

### Phase 2 — Causal Research Design

#### Day 16 — Dataset Documentation and Causal Design

**Work completed:**

* Reviewed dataset structure.
* Investigated available variables.
* Studied potential causal research questions.
* Assessed preliminary causal research feasibility.
* Documented research limitations.

**Output:**

* `day16_causal_research_design_assessment.csv`

#### Day 17 — Treatment Definition and Identification Strategy

**Work completed:**

* Evaluated potential treatment variables.
* Investigated treatment assignment and campaign exposure.
* Examined potential outcome variables.
* Assessed causal identification requirements.
* Documented unresolved assumptions.

**Outputs:**

* `day17_treatment_candidate_assessment.csv`
* `day17_causal_identification_assessment.csv`
* `day17_causal_research_assessment.csv`

**Key finding:**

Actual campaign exposure and a sufficiently defensible treatment assignment mechanism have not yet been established.

#### Day 18 — Dataset Documentation Research

**Work completed:**

* Investigated original dataset documentation.
* Studied transaction variables.
* Examined extreme transaction quantities.
* Investigated Fuel category transaction patterns.
* Analyzed frequently observed Fuel items.
* Compared price-to-quantity ratios.
* Documented measurement limitations.

**Output:**

* `day18_fuel_item_analysis.csv`

**Key finding:**

Six frequently observed Fuel items showed relatively consistent price-to-quantity ratios, with a mean of approximately 0.086807.

#### Day 19 — Transaction Outcome Validation

**Work completed:**

* Inspected transaction columns and data types.
* Checked missing values and duplicates.
* Investigated transaction date coverage.
* Analyzed quantity and selling price.
* Examined other and coupon discounts.
* Investigated item-level price variation.
* Compared preliminary expenditure candidates.
* Aggregated transactions at customer level.
* Analyzed customer spending distributions.
* Investigated spending concentration.
* Exported and verified customer-level analysis.

**Output:**

* `day19_customer_spending_analysis.csv`

**Key finding:**

Customer-level aggregation provides exploratory spending measures, but the exact definitions of quantity, selling price, and discounts require further validation.

#### Day 20 — Transaction Measurement Verification and Outcome Feasibility

**Work completed:**

* Investigated transaction variable definitions.
* Examined selling price and quantity relationships.
* Analyzed discount measurement patterns.
* Compared recorded and adjusted amounts.
* Investigated product category differences.
* Examined customer-level discount impact.
* Compared customers with and without recorded coupon discounts.
* Assessed customer-level outcome feasibility.
* Documented the final research recommendation.

**Outputs:**

* `20_transaction_measurement_outcome_feasibility.ipynb`
* `DAY20_REPORT.md`
* `day20_outcome_feasibility_assessment.csv`

**Key finding:**

Customer-level expenditure analysis is technically possible, but the actual expenditure measurement convention has not been sufficiently verified.

**Outcome feasibility decision: PARTIALLY FEASIBLE**

Neither preliminary expenditure candidate has yet been established as a validated causal outcome.

## 7. Causal Research Framework

The project follows an important principle:

**Prediction does not automatically imply causation.**

Before estimating campaign effects, the research must establish:

1. A clearly defined treatment or intervention.
2. A defensible treatment assignment mechanism.
3. A properly measured outcome.
4. Relevant pre-treatment confounders.
5. Appropriate identification assumptions.
6. Sufficient treatment overlap.

### Treatment Considerations

`redemption_status` is a potential outcome candidate, but coupon redemption does not independently establish campaign exposure or treatment assignment.

Campaign types X and Y are anonymized categories and should not automatically be interpreted as treatment and control groups.

### Outcome Considerations

Customer transaction data provides information about purchasing behaviour.

However, the definitions and measurement conventions of `quantity`, `selling_price`, `other_discount`, and `coupon_discount` must be verified before selecting a reliable expenditure outcome.

### Double Machine Learning

Double Machine Learning combines machine learning methods with statistical techniques to estimate causal effects under appropriate identification assumptions.

It does not independently solve:

* Unobserved confounding.
* Incorrect treatment definitions.
* Invalid outcome measurement.
* Unreliable treatment assignment.
* Lack of treatment overlap.

## 8. Technology Stack

| Technology   | Purpose                      |
| ------------ | ---------------------------- |
| Python       | Programming language         |
| JupyterLab   | Research and experimentation |
| NumPy        | Numerical computations       |
| Pandas       | Data manipulation            |
| Matplotlib   | Data visualization           |
| Seaborn      | Statistical visualization    |
| Scikit-learn | Machine learning             |
| Git          | Version control              |
| GitHub       | Project documentation        |

## 9. Current Research Limitations

* Actual campaign exposure remains unresolved.
* Treatment assignment mechanism is not established.
* Campaign type labels are anonymized.
* Customer demographic information is not available for every training record.
* Transaction quantity units require further documentation.
* Selling price measurement conventions remain uncertain.
* Discount calculation conventions need verification.
* A validated customer-level expenditure outcome has not yet been established.
* Causal identification assumptions require further investigation.

## 10. Next Research Phase — Causal Identification and DML Feasibility

The original 20-day project plan has been completed.

The next phase will focus on:

1. Original transaction variable documentation.
2. Customer-level outcome validation.
3. Actual campaign exposure investigation.
4. Treatment assignment mechanism.
5. Confounding variable identification.
6. Treatment and control group overlap.
7. Causal identification strategy.
8. Double Machine Learning feasibility.
9. Causal estimation, if identification is justified.
10. Robustness and sensitivity analysis.

## 11. Project Status

| Milestone                                   | Status      |
| ------------------------------------------- | ----------- |
| Initial data analysis (Days 1–15)           | Completed   |
| Dataset documentation (Day 16)              | Completed   |
| Treatment definition assessment (Day 17)    | Completed   |
| Transaction documentation research (Day 18) | Completed   |
| Transaction outcome validation (Day 19)     | Completed   |
| Outcome feasibility assessment (Day 20)     | Completed   |
| Final outcome validation                    | In progress |
| Causal identification                       | Pending     |
| DML feasibility                             | Pending     |
| DML estimation                              | Pending     |

## 12. Conclusion

EconoCausal aims to develop a reliable causal machine learning framework for understanding the effects of promotional campaigns on customer purchasing behaviour.

The first 20 days established a foundation in dataset understanding, transaction analysis, treatment investigation, and outcome feasibility.

The next phase will focus on establishing a scientifically defensible treatment, outcome, and identification strategy before attempting Double Machine Learning estimation.

## 13. Author

Developed as part of a Data Science internship project.

**Project:** EconoCausal
**Research Focus:** Dynamic Pricing and Causal Analysis Using Double Machine Learning
**Current Progress:** Day 20 Completed
