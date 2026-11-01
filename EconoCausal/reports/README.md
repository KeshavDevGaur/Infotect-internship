# EconoCausal — Reports and Research Outputs

This directory contains research reports, analytical summaries, assessment files, and exported results generated during the EconoCausal project.

Each report documents research activities, findings, assumptions, limitations, and analytical outputs produced during the corresponding project phase.

## 1. Project Information

**Project:** EconoCausal

**Research Focus:** Dynamic Pricing and Causal Analysis Using Double Machine Learning

**Dataset:** AmExpert 2019 Marketing Campaign

**Programming Language:** Python

## 2. Report Organization

| Day    | Report            | Research Focus                                   |
| ------ | ----------------- | ------------------------------------------------ |
| Day 16 | `DAY16_REPORT.md` | Dataset documentation and causal design          |
| Day 17 | `DAY17_REPORT.md` | Treatment definition and identification strategy |
| Day 18 | `DAY18_REPORT.md` | Dataset documentation and transaction research   |
| Day 19 | `DAY19_REPORT.md` | Transaction outcome validation                   |
| Day 20 | `DAY20_REPORT.md` | Transaction measurement and outcome feasibility  |

## 3. Detailed Report Documentation

### Day 16 — Dataset Documentation and Causal Design

**Report:**

`DAY16_REPORT.md`

**Assessment file:**

* `day16_causal_research_design_assessment.csv`

**Work completed:**

* Reviewed the original dataset structure.
* Investigated available variables.
* Studied customer and campaign information.
* Identified potential causal research questions.
* Assessed preliminary causal research feasibility.
* Documented initial research limitations.

**Objective:**

Establish an initial understanding of the dataset and identify requirements for developing a defensible causal research design.

### Day 17 — Treatment Definition and Identification Strategy

**Report:**

`DAY17_REPORT.md`

**Assessment files:**

* `day17_treatment_candidate_assessment.csv`
* `day17_causal_identification_assessment.csv`
* `day17_causal_research_assessment.csv`

**Work completed:**

* Evaluated potential treatment variables.
* Investigated treatment assignment.
* Examined possible campaign exposure.
* Evaluated potential outcome variables.
* Assessed causal identification assumptions.
* Documented unresolved research limitations.

**Key finding:**

The available dataset does not yet establish actual campaign exposure or a sufficiently defensible treatment assignment mechanism.

**Conclusion:**

Further investigation is required before defining treatment and control groups for causal estimation.

### Day 18 — Dataset Documentation Research

**Report:**

`DAY18_REPORT.md`

**Assessment file:**

* `day18_fuel_item_analysis.csv`

**Work completed:**

**1. Original Dataset Research**

* Investigated original dataset documentation.
* Examined campaign and coupon characteristics.
* Reviewed relevant published causal marketing research.

**2. Transaction Data Investigation**

* Examined transaction-level variables.
* Investigated quantity and selling price.
* Analyzed discount variables.
* Examined transaction distributions.

**3. Extreme Quantity Investigation**

* Identified unusually large quantities.
* Compared product category transaction patterns.
* Investigated frequently observed Fuel items.

**4. Fuel Item Analysis**

* Investigated item 49009.
* Compared other frequently observed Fuel items.
* Examined price-to-quantity ratios.
* Evaluated consistency across selected items.

**Key finding:**

Six frequently observed Fuel items showed relatively consistent price-to-quantity ratios, with a mean of approximately 0.086807.

**Conclusion:**

Transaction measurement conventions require further documentation before constructing a reliable customer expenditure outcome.

### Day 19 — Transaction Outcome Validation

**Report:**

`DAY19_REPORT.md`

**Assessment file:**

* `day19_customer_spending_analysis.csv`

**Work completed:**

**1. Transaction Data Inspection**

* Inspected transaction columns and data types.
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
* Compared recorded and discount-adjusted amounts.

**4. Expenditure Candidate Investigation**

Compared two preliminary expenditure candidates:

Candidate A:

`selling_price`

Candidate B:

`selling_price + other_discount + coupon_discount`

Neither candidate has been established as the actual customer expenditure measure.

**5. Customer-Level Analysis**

* Aggregated transaction records by customer.
* Calculated transaction counts and quantity totals.
* Calculated recorded and adjusted spending candidates.
* Investigated spending distributions.
* Identified customers with extreme spending.
* Analyzed spending concentration.
* Examined transaction frequency and spending relationships.

**6. Validation and Export**

* Checked customer-level missing values.
* Investigated zero and negative values.
* Exported customer-level analysis.
* Reloaded the CSV to verify the output.

**Key finding:**

Customer-level transaction aggregation provides exploratory spending measures, but the underlying variable definitions require further validation.

**Conclusion:**

Neither preliminary expenditure candidate has yet been validated as a reliable causal outcome.

### Day 20 — Transaction Measurement Verification and Outcome Feasibility

**Report:**

`DAY20_REPORT.md`

**Assessment file:**

* `day20_outcome_feasibility_assessment.csv`

**Work completed:**

**1. Transaction Variable Investigation**

* Investigated original transaction columns.
* Examined data types.
* Documented variables requiring verification.

**2. Selling Price and Quantity Investigation**

* Examined frequently observed items.
* Investigated selling price variation.
* Studied quantity-price relationships.
* Examined individual item transaction patterns.
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

**Key finding:**

Customer-level expenditure analysis is technically possible, but actual expenditure measurement conventions have not been sufficiently verified.

**Outcome feasibility decision: PARTIALLY FEASIBLE.**

Neither preliminary expenditure candidate has yet been established as a validated causal outcome.

**Conclusion:**

Further transaction documentation and causal research are required before proceeding with Double Machine Learning estimation.

## 4. Output File Descriptions

| File                                          | Description                                               |
| --------------------------------------------- | --------------------------------------------------------- |
| `DAY16_REPORT.md`                             | Day 16 research summary                                   |
| `DAY17_REPORT.md`                             | Day 17 research summary                                   |
| `DAY18_REPORT.md`                             | Day 18 research summary                                   |
| `DAY19_REPORT.md`                             | Day 19 research summary                                   |
| `DAY20_REPORT.md`                             | Day 20 research summary                                   |
| `day16_causal_research_design_assessment.csv` | Preliminary causal research assessment                    |
| `day17_treatment_candidate_assessment.csv`    | Evaluation of potential treatment variables               |
| `day17_causal_identification_assessment.csv`  | Causal identification assessment                          |
| `day17_causal_research_assessment.csv`        | Overall causal research assessment                        |
| `day18_fuel_item_analysis.csv`                | Analysis of frequently observed Fuel items                |
| `day19_customer_spending_analysis.csv`        | Customer-level transaction and spending analysis          |
| `day20_outcome_feasibility_assessment.csv`    | Preliminary customer-level outcome feasibility assessment |

## 5. Research Documentation Standards

All reports and analytical outputs should follow these principles:

1. Clearly document the research objective.
2. Describe the dataset and variables used.
3. Explain the analytical methodology.
4. Document important findings.
5. Identify assumptions and limitations.
6. Avoid unsupported interpretations.
7. Maintain reproducibility.
8. Separate descriptive associations from causal conclusions.
9. Document output files and their purposes.
10. Preserve the distinction between campaign exposure and coupon redemption.

## 6. Important Causal Research Considerations

The project aims to investigate promotional campaign effects using Double Machine Learning.

However, reliable causal estimation requires a defensible research design.

The following issues remain important:

* Actual campaign exposure.
* Treatment assignment mechanism.
* Valid treatment and control definitions.
* Proper outcome measurement.
* Confounding variables.
* Treatment overlap.
* Identification assumptions.

The existence of a redemption variable does not independently establish campaign exposure or treatment assignment.

Similarly, customer-level spending aggregates do not automatically represent valid causal outcomes.

## 7. Upcoming Research Reports

Future reports may include:

| Planned Research                | Objective                                                             |
| ------------------------------- | --------------------------------------------------------------------- |
| Transaction Variable Validation | Verify transaction variable definitions and measurement units         |
| Outcome Feasibility Assessment  | Establish whether customer-level expenditure can be reliably measured |
| Campaign Exposure Assessment    | Investigate actual campaign exposure                                  |
| Treatment Assignment Analysis   | Evaluate how customers received campaign offers                       |
| Confounding Assessment          | Identify relevant pre-treatment confounders                           |
| Overlap Assessment              | Investigate treatment and control group overlap                       |
| DML Feasibility Assessment      | Determine whether Double Machine Learning is appropriate              |
| Causal Estimation Report        | Document justified causal estimates, if feasible                      |
| Robustness Analysis             | Evaluate the stability of results                                     |

## 8. Project Status

| Research Phase                              | Status      |
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

## 9. Conclusion

The reports directory provides a structured record of the EconoCausal research workflow.

The first 20 days established a foundation for dataset understanding, treatment investigation, transaction analysis, and preliminary customer-level outcome construction.

The outcome feasibility assessment concluded that customer-level expenditure analysis is technically possible, but the actual expenditure measurement convention remains insufficiently verified.

The next phase will focus on establishing a defensible treatment, outcome, and identification strategy before proceeding with Double Machine Learning estimation.

---

**Project:** EconoCausal

**Original Project Plan:** 20 Days

**Current Progress:** Day 20 Completed

**Next Focus:** Causal Identification and DML Feasibility
