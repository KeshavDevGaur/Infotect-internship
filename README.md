# EconoCausal

### Dynamic Pricing and Causal Analysis Using Double Machine Learning

![Python](https://img.shields.io/badge/Python-3.x-blue)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-yellow)
![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-orange)
![Status](https://img.shields.io/badge/Progress-Day%2019-success)

## 1. Project Overview

EconoCausal is a data science research project focused on understanding customer purchasing behaviour, promotional campaigns, discounts, and the feasibility of causal analysis using the AmExpert 2019 Marketing Campaign dataset.

The project investigates how promotional campaigns and discounts may influence customer purchasing behaviour.

The long-term objective is to evaluate whether Double Machine Learning (DML) can provide reliable estimates of promotional campaign effects.

The project emphasizes data quality, treatment definition, outcome construction, and causal identification before model estimation.

## 2. Research Objectives

* Explore customer purchasing behaviour.
* Understand promotional campaign characteristics.
* Analyze coupon and transaction information.
* Investigate customer-level spending patterns.
* Identify potential treatment and outcome variables.
* Evaluate treatment assignment and campaign exposure.
* Investigate confounding and identification assumptions.
* Assess the feasibility of Double Machine Learning.
* Develop a reproducible causal research workflow.

## 3. Dataset Information

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

## 4. Project Structure

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
│   └── README.md
│
├── reports/
│   ├── DAY16_REPORT.md
│   ├── DAY17_REPORT.md
│   ├── DAY18_REPORT.md
│   ├── DAY19_REPORT.md
│   ├── day16_causal_research_design_assessment.csv
│   ├── day17_treatment_candidate_assessment.csv
│   ├── day17_causal_identification_assessment.csv
│   ├── day17_causal_research_assessment.csv
│   ├── day18_fuel_item_analysis.csv
│   ├── day19_customer_spending_analysis.csv
│   └── README.md
│
└── README.md
```

## 5. Research Progress

### Phase 1 — Initial Data Analysis (Days 1–15)

Completed the initial project workflow, including dataset exploration, data preparation, descriptive analysis, and preliminary research.

The first 15 days established the foundation for understanding the dataset and investigating customer and campaign information.

### Phase 2 — Causal Research Design

#### Day 16 — Dataset Documentation and Causal Design

**Work completed:**

* Reviewed dataset structure.
* Investigated available variables.
* Studied potential causal research questions.
* Assessed preliminary causal research feasibility.
* Documented research design limitations.

**Output:**

* `day16_causal_research_design_assessment.csv`

#### Day 17 — Treatment Definition and Identification Strategy

**Work completed:**

* Evaluated potential treatment variables.
* Investigated treatment assignment and exposure.
* Examined possible outcome variables.
* Assessed causal identification requirements.
* Documented unresolved assumptions.

**Outputs:**

* `day17_treatment_candidate_assessment.csv`
* `day17_causal_identification_assessment.csv`
* `day17_causal_research_assessment.csv`

**Key finding:**

The available information does not yet establish actual campaign exposure or a sufficiently defensible treatment assignment mechanism.

#### Day 18 — Dataset Documentation Research

**Work completed:**

* Investigated original dataset documentation.
* Studied transaction variable distributions.
* Examined extreme transaction quantities.
* Investigated Fuel category transaction patterns.
* Analyzed frequently observed Fuel items.
* Compared price-to-quantity ratios.
* Documented transaction measurement limitations.

**Output:**

* `day18_fuel_item_analysis.csv`

**Key finding:**

Six frequently observed Fuel items showed relatively consistent price-to-quantity ratios, with a mean of approximately 0.086807.

**Conclusion:**

Transaction measurement conventions require further investigation before constructing a reliable customer expenditure outcome.

#### Day 19 — Transaction Outcome Validation

**Work completed:**

* Inspected transaction columns and data types.
* Checked missing values and duplicate records.
* Investigated transaction date coverage.
* Analyzed quantity and selling price distributions.
* Examined other and coupon discounts.
* Investigated item-level price variation.
* Compared preliminary expenditure candidates.
* Aggregated transactions at customer level.
* Analyzed customer spending distributions.
* Investigated spending concentration among the top 10% of customers.
* Examined the relationship between transaction frequency and spending.
* Exported and verified customer-level analysis.

**Outputs:**

* `19_transaction_outcome_validation.ipynb`
* `day19_customer_spending_analysis.csv`
* `DAY19_REPORT.md`

**Key finding:**

Customer-level transaction aggregation provides exploratory spending measures. However, the exact definitions of quantity, selling price, and discounts require further validation.

**Conclusion:**

Neither preliminary expenditure candidate has yet been validated as the actual customer expenditure outcome.

## 6. Causal Research Framework

The project follows an important principle:

**Prediction does not automatically imply causation.**

Before estimating campaign effects, the research must establish:

1. A clearly defined treatment or intervention.
2. A defensible treatment assignment mechanism.
3. A properly measured outcome variable.
4. Relevant pre-treatment confounders.
5. Appropriate identification assumptions.
6. Sufficient data quality and treatment overlap.

### Treatment Considerations

The `redemption_status` variable is a potential outcome candidate, but coupon redemption does not establish actual campaign exposure or treatment assignment.

Campaign types X and Y are anonymized categories and should not automatically be interpreted as treatment and control groups.

### Outcome Considerations

Customer transaction data provides information about purchasing behaviour.

However, the exact meanings of `quantity`, `selling_price`, `other_discount`, and `coupon_discount` must be established before selecting a reliable expenditure measure.

### Double Machine Learning

Double Machine Learning combines machine learning techniques with statistical methods to estimate causal effects under suitable identification assumptions.

It does not independently solve problems involving:

* Unobserved confounding.
* Incorrect treatment definitions.
* Invalid outcome measurements.
* Unreliable treatment assignment.
* Lack of treatment overlap.

## 7. Technology Stack

| Technology   | Purpose                                 |
| ------------ | --------------------------------------- |
| Python       | Main programming language               |
| JupyterLab   | Research and experimentation            |
| NumPy        | Numerical computations                  |
| Pandas       | Data manipulation and analysis          |
| Matplotlib   | Data visualization                      |
| Seaborn      | Statistical visualization               |
| Scikit-learn | Machine learning                        |
| Git          | Version control                         |
| GitHub       | Project documentation and collaboration |

## 8. Current Research Limitations

* Actual campaign exposure has not yet been established.
* Treatment assignment mechanism remains unresolved.
* Campaign type labels are anonymized.
* Customer demographic information is not available for every training record.
* Transaction quantity units require further documentation.
* The meaning of selling price needs verification.
* Discount calculation conventions remain unconfirmed.
* A defensible customer-level expenditure outcome is still under investigation.
* Causal identification assumptions require additional verification.

## 9. Future Work

### Day 20 and Upcoming Research

* Investigate original transaction variable definitions.
* Verify the meaning and units of quantity.
* Validate selling price and discount calculations.
* Assess customer-level outcome feasibility.
* Investigate campaign exposure and treatment assignment.
* Evaluate potential confounding variables.
* Examine treatment overlap.
* Finalize the causal research design.
* Assess Double Machine Learning feasibility.
* Conduct estimation only after identification assumptions are justified.
* Perform robustness and sensitivity analysis.

## 10. Research Principles

This project follows these principles:

* Reproducible analysis.
* Clear documentation.
* Proper data validation.
* Transparent assumptions.
* Separation of correlation and causation.
* No unsupported interpretation of anonymized variables.
* No premature causal estimation.

## 11. Project Status

| Milestone                                        | Status      |
| ------------------------------------------------ | ----------- |
| Initial dataset exploration (Days 1–15)          | Completed   |
| Dataset documentation and causal design (Day 16) | Completed   |
| Treatment definition assessment (Day 17)         | Completed   |
| Transaction documentation research (Day 18)      | Completed   |
| Transaction outcome validation (Day 19)          | Completed   |
| Outcome feasibility assessment                   | In progress |
| Causal identification                            | In progress |
| DML estimation                                   | Pending     |

**Current Progress: Day 19 Completed**

## 12. Author

Developed as part of a Data Science internship project.

**Project Name:** EconoCausal
**Research Focus:** Dynamic Pricing and Causal Analysis Using Double Machine Learning
