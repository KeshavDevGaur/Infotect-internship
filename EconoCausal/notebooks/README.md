# EconoCausal — Jupyter Notebooks

This directory contains the Jupyter notebooks developed during the EconoCausal research project.

The notebooks document the complete analytical workflow, including dataset exploration, data preparation, transaction analysis, research design, treatment definition, outcome validation, and causal machine learning feasibility.

## 1. Project Overview

**Project:** EconoCausal

**Research Focus:** Dynamic Pricing and Causal Analysis Using Double Machine Learning

**Dataset:** AmExpert 2019 Marketing Campaign

**Primary Language:** Python

**Environment:** JupyterLab / Jupyter Notebook

## 2. Notebook Organization

The notebooks are organized chronologically according to the project development timeline.

| Period         | Focus                                                  | Status    |
| -------------- | ------------------------------------------------------ | --------- |
| Days 1–15      | Initial dataset exploration, preparation, and analysis | Completed |
| Day 16         | Dataset documentation and causal design                | Completed |
| Day 17         | Treatment definition and identification strategy       | Completed |
| Day 18         | Dataset documentation research                         | Completed |
| Day 19         | Transaction outcome validation                         | Completed |
| Day 20 onwards | Further outcome and causal research                    | Upcoming  |

## 3. Detailed Notebook Documentation

### Day 01–15 — Initial Data Analysis

These notebooks establish the foundation of the EconoCausal project.

The initial project phase focuses on understanding the dataset, investigating customer and campaign information, preparing analytical data, and conducting exploratory analysis.

**General objectives:**

* Understand the dataset structure.
* Explore available variables.
* Perform data inspection and preparation.
* Investigate customer and transaction information.
* Conduct exploratory data analysis.
* Document analytical observations.

Refer to the individual daily notebooks for the detailed implementation and results.

### Day 16 — Dataset Documentation and Causal Design

**Notebook:**

`16_dataset_documentation_causal_design.ipynb`

**Objectives:**

* Understand the original dataset structure.
* Investigate campaign and customer information.
* Identify potential causal research questions.
* Examine available treatment and outcome candidates.
* Assess preliminary causal research feasibility.

**Work completed:**

* Dataset documentation.
* Variable investigation.
* Research question development.
* Preliminary causal design assessment.
* Identification of research limitations.

**Output:**

`day16_causal_research_design_assessment.csv`

### Day 17 — Treatment Definition and Identification Strategy

**Notebook:**

`17_treatment_definition_identification_strategy.ipynb`

**Objectives:**

* Identify potential treatment variables.
* Investigate treatment assignment.
* Examine campaign exposure.
* Evaluate potential outcome variables.
* Assess causal identification requirements.

**Work completed:**

1. Treatment candidate evaluation.
2. Treatment and control group investigation.
3. Outcome candidate assessment.
4. Treatment assignment analysis.
5. Causal identification assessment.
6. Documentation of unresolved assumptions.

**Outputs:**

* `day17_treatment_candidate_assessment.csv`
* `day17_causal_identification_assessment.csv`
* `day17_causal_research_assessment.csv`

**Key finding:**

The available dataset does not yet establish actual campaign exposure or a sufficiently defensible treatment assignment mechanism.

### Day 18 — Dataset Documentation Research

**Notebook:**

`18_dataset_documentation_research.ipynb`

**Objectives:**

* Investigate original dataset documentation.
* Understand transaction variables.
* Examine unusual transaction quantities.
* Investigate Fuel category purchasing patterns.
* Assess transaction measurement limitations.

**Work completed:**

**1. Original Dataset Research**

* Reviewed original dataset documentation.
* Investigated campaign and coupon characteristics.
* Reviewed relevant published causal marketing research.

**2. Transaction Data Investigation**

* Examined transaction variables.
* Investigated quantity and selling price.
* Analyzed discount variables.
* Examined variable distributions.

**3. Extreme Quantity Investigation**

* Identified unusually large transaction quantities.
* Compared transaction quantities across product categories.
* Investigated frequently observed Fuel items.

**4. Fuel Item Analysis**

* Investigated item 49009.
* Compared other frequently observed Fuel items.
* Calculated price-to-quantity ratios.
* Examined ratio consistency.

**Output:**

`day18_fuel_item_analysis.csv`

**Key finding:**

Six frequently observed Fuel items showed relatively consistent price-to-quantity ratios, with a mean of approximately 0.086807.

**Conclusion:**

Transaction measurement conventions require further investigation before constructing a reliable customer expenditure outcome.

### Day 19 — Transaction Outcome Validation

**Notebook:**

`19_transaction_outcome_validation.ipynb`

**Objectives:**

* Investigate transaction-level variables.
* Analyze quantity and selling price.
* Examine discount calculations.
* Compare preliminary expenditure candidates.
* Aggregate transactions at customer level.
* Evaluate customer-level spending patterns.

**Work completed:**

**1. Transaction Data Inspection**

* Inspected column names and data types.
* Checked missing values.
* Checked duplicate records.
* Investigated transaction date coverage.

**2. Quantity and Selling Price Analysis**

* Examined statistical distributions.
* Investigated extreme quantity values.
* Studied the relationship between quantity and selling price.
* Calculated provisional price-per-quantity ratios.
* Investigated item-level price variation.

**3. Discount Analysis**

* Examined `other_discount`.
* Examined `coupon_discount`.
* Investigated discount combinations.
* Compared recorded and discount-adjusted amounts.

**4. Customer-Level Aggregation**

Created customer-level measures:

* Total transactions.
* Total quantity.
* Total recorded selling price.
* Total adjusted amount.
* Total other discount.
* Total coupon discount.

**5. Customer Spending Analysis**

* Examined customer-level spending distributions.
* Investigated customers with extreme spending.
* Calculated spending percentiles.
* Investigated spending concentration among the top 10% of customers.
* Analyzed transaction frequency and spending.
* Compared spending across transaction-frequency groups.

**6. Outcome Validation**

* Compared expenditure candidates.
* Checked missing values.
* Investigated zero and negative values.
* Exported customer-level analysis.
* Verified the exported CSV.

**Output:**

`day19_customer_spending_analysis.csv`

**Key finding:**

Customer-level aggregation provides exploratory spending measures. However, the exact definitions of quantity, selling price, and discounts require further validation.

**Conclusion:**

Neither preliminary expenditure candidate has yet been validated as the actual customer expenditure outcome.

## 4. Notebook Execution Guidelines

Follow these guidelines when working with the notebooks:

1. Execute notebook cells sequentially.
2. Import required libraries before using them.
3. Use relative file paths.
4. Keep the original raw datasets unchanged.
5. Document important analytical findings.
6. Include appropriate visualizations.
7. Validate calculations before interpreting results.
8. Export important analytical outputs into the reports directory.
9. Avoid removing extreme values without investigation.
10. Clearly distinguish descriptive analysis from causal conclusions.

## 5. Technologies and Libraries

| Library      | Purpose                          |
| ------------ | -------------------------------- |
| NumPy        | Numerical computations           |
| Pandas       | Data manipulation                |
| Matplotlib   | Data visualization               |
| Seaborn      | Statistical visualization        |
| Scikit-learn | Machine learning                 |
| JupyterLab   | Interactive research environment |

## 6. Expected Future Notebook Work

Upcoming notebooks will investigate:

* Transaction variable definitions.
* Quantity and selling price measurement.
* Discount calculation conventions.
* Customer-level outcome feasibility.
* Campaign exposure.
* Treatment assignment.
* Confounding variables.
* Treatment overlap.
* Double Machine Learning feasibility.
* Causal effect estimation.
* Robustness and sensitivity analysis.

## 7. Important Research Note

Double Machine Learning should not be applied merely because treatment and outcome columns are available.

A defensible causal analysis requires:

* A clearly defined treatment.
* A properly measured outcome.
* A justified identification strategy.
* Appropriate confounder adjustment.
* Sufficient treatment overlap.

The notebooks document these requirements as part of the research workflow.

---

**Project:** EconoCausal

**Current Progress:** Day 19 Completed

**Next Focus:** Transaction measurement verification and outcome feasibility assessment.
