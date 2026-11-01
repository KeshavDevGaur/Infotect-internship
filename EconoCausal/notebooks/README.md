# EconoCausal — Jupyter Notebooks

This directory contains the Jupyter notebooks developed during the EconoCausal research project.

The notebooks document the analytical workflow, including dataset exploration, data preparation, transaction analysis, research design, treatment definition, outcome validation, and causal machine learning feasibility.

## 1. Project Information

**Project:** EconoCausal

**Research Focus:** Dynamic Pricing and Causal Analysis Using Double Machine Learning

**Dataset:** AmExpert 2019 Marketing Campaign

**Programming Language:** Python

**Environment:** JupyterLab / Jupyter Notebook

## 2. Notebook Organization

| Period    | Research Focus                                   | Status    |
| --------- | ------------------------------------------------ | --------- |
| Days 1–15 | Initial dataset exploration and preparation      | Completed |
| Day 16    | Dataset documentation and causal design          | Completed |
| Day 17    | Treatment definition and identification strategy | Completed |
| Day 18    | Dataset documentation research                   | Completed |
| Day 19    | Transaction outcome validation                   | Completed |
| Day 20    | Transaction measurement and outcome feasibility  | Completed |

## 3. Detailed Notebook Documentation

### Days 01–15 — Initial Data Analysis

These notebooks establish the foundation of the EconoCausal project.

**General objectives:**

* Understand dataset structure.
* Explore available variables.
* Perform data inspection and preparation.
* Investigate customer and transaction information.
* Conduct exploratory data analysis.
* Document analytical observations.

Refer to the individual daily notebooks for detailed implementation and results.

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

Actual campaign exposure and a sufficiently defensible treatment assignment mechanism have not yet been established.

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

* Inspected columns and data types.
* Checked missing values and duplicate records.
* Investigated transaction date coverage.

**2. Quantity and Selling Price Analysis**

* Examined statistical distributions.
* Investigated extreme quantity values.
* Studied quantity and selling price relationships.
* Examined item-level price variation.

**3. Discount Analysis**

* Investigated `other_discount`.
* Investigated `coupon_discount`.
* Analyzed discount combinations.
* Compared recorded and adjusted amounts.

**4. Customer-Level Aggregation**

Created customer-level measures:

* Total transactions.
* Total quantity.
* Total recorded selling price.
* Total adjusted amount.
* Total other discount.
* Total coupon discount.

**5. Customer Spending Analysis**

* Examined spending distributions.
* Investigated customers with extreme spending.
* Calculated spending percentiles.
* Investigated spending concentration.
* Analyzed transaction frequency and spending.

**6. Outcome Validation**

* Compared expenditure candidates.
* Checked missing values.
* Investigated zero and negative values.
* Exported and verified customer-level analysis.

**Output:**

`day19_customer_spending_analysis.csv`

**Key finding:**

Customer-level aggregation provides exploratory spending measures, but transaction measurement conventions require further verification.

### Day 20 — Transaction Measurement Verification and Outcome Feasibility

**Notebook:**

`20_transaction_measurement_outcome_feasibility.ipynb`

**Objectives:**

* Investigate transaction variable definitions.
* Examine selling price and quantity relationships.
* Verify discount measurement patterns.
* Compare expenditure candidates.
* Investigate category-level transaction patterns.
* Assess customer-level outcome feasibility.

**Work completed:**

**1. Transaction Variable Investigation**

* Inspected original transaction columns.
* Examined data types.
* Documented variables requiring verification.

**2. Selling Price and Quantity Investigation**

* Examined frequently observed items.
* Investigated selling price variation.
* Studied quantity-price relationships.
* Examined individual item patterns.
* Calculated provisional amount-per-quantity measures.

**3. Discount Measurement Investigation**

* Analyzed negative, zero, and positive discount values.
* Examined discount patterns across products.
* Compared recorded and adjusted amounts.
* Investigated negative and zero adjusted amounts.

**4. Product Category Investigation**

* Combined transaction data with item metadata.
* Compared quantity and selling price relationships.
* Examined adjusted amounts across categories.
* Investigated unusual category-level values.

**5. Customer-Level Analysis**

* Aggregated transactions by customer.
* Investigated customer-level discount impact.
* Compared customers with and without recorded coupon discounts.

**6. Outcome Feasibility Assessment**

* Evaluated customer-level aggregation.
* Investigated expenditure measurement limitations.
* Assessed whether available measures were ready for causal analysis.
* Documented the final research recommendation.

**Expected outputs:**

* `DAY20_REPORT.md`
* `day20_outcome_feasibility_assessment.csv`

**Key finding:**

Customer-level expenditure analysis is technically possible, but actual expenditure measurement conventions have not been sufficiently verified.

**Outcome feasibility decision: PARTIALLY FEASIBLE.**

Neither preliminary expenditure candidate is yet a validated causal outcome.

## 4. Notebook Execution Guidelines

1. Execute notebook cells sequentially.
2. Import required libraries before using them.
3. Use relative file paths.
4. Keep original raw datasets unchanged.
5. Document important findings.
6. Include appropriate visualizations.
7. Validate calculations before interpretation.
8. Export analytical results into the reports directory.
9. Investigate extreme values before removing them.
10. Separate descriptive analysis from causal conclusions.

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

The next research phase will focus on:

* Original transaction variable documentation.
* Customer-level outcome validation.
* Campaign exposure investigation.
* Treatment assignment mechanism.
* Confounding variable identification.
* Treatment overlap.
* Causal identification strategy.
* Double Machine Learning feasibility.
* Causal effect estimation, if justified.
* Robustness and sensitivity analysis.

## 7. Important Research Note

Double Machine Learning should not be applied merely because treatment and outcome columns are available.

A defensible causal analysis requires:

* Clearly defined treatment.
* Properly measured outcome.
* Justified identification strategy.
* Appropriate confounder adjustment.
* Sufficient treatment overlap.

The notebooks document these requirements throughout the project.

---

**Project:** EconoCausal

**Original Project Plan:** 20 Days

**Current Progress:** Day 20 Completed

**Next Focus:** Causal Identification and DML Feasibility
