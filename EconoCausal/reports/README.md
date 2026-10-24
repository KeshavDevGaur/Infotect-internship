# EconoCausal — Reports and Analysis Outputs

This directory contains daily project reports and CSV files generated during the EconoCausal project.

The reports document data exploration, data quality checks, customer and campaign relationships, and preliminary causal inference assessments.

## Daily Reports

| Report            | Description                                         |
| ----------------- | --------------------------------------------------- |
| `DAY1_REPORT.md`  | Initial dataset inspection                          |
| `DAY2_REPORT.md`  | Data quality and duplicate analysis                 |
| `DAY3_REPORT.md`  | Dataset relationship validation                     |
| `DAY4_REPORT.md`  | Target and campaign analysis                        |
| `DAY5_REPORT.md`  | Customer demographics and coupon analysis           |
| `DAY6_REPORT.md`  | Transaction and discount analysis                   |
| `DAY7_REPORT.md`  | Dataset integration and causal variable exploration |
| `DAY8_REPORT.md`  | Preliminary causal feasibility assessment           |
| `DAY9_REPORT.md`  | Campaign exposure investigation                     |
| `DAY10_REPORT.md` | Customer-campaign relationship analysis             |
| `DAY11_REPORT.md` | Treatment and outcome assessment                    |
| `DAY12_REPORT.md` | Treatment assignment assessment                     |
| `DAY13_REPORT.md` | Customer-level treatment and exposure investigation |

## Analysis Output Files

The directory may contain the following CSV outputs, provided they have been generated and saved.

### Days 1–3: Data Exploration and Quality

* `day01_dataset_summary.csv`
* `day02_duplicate_analysis.csv`
* `day02_missing_values.csv`
* `day03_relationship_validation.csv`
* `day03_training_structure.csv`

### Days 4–5: Target, Campaign, Customer, and Coupon Analysis

* `day04_campaign_redemption.csv`
* `day04_campaign_type_analysis.csv`
* `day04_top_campaigns.csv`
* `day05_age_redemption.csv`
* `day05_marital_redemption.csv`
* `day05_income_redemption.csv`
* `day05_coupon_item_counts.csv`
* `day05_category_counts.csv`

### Days 6–7: Transactions and Dataset Integration

* `day06_transaction_summary.csv`
* `day06_missing_values.csv`
* `day06_duplicate_analysis.csv`
* `day06_discount_correlation.csv`
* `day07_integration_summary.csv`
* `day07_causal_variable_summary.csv`

### Days 8–10: Preliminary Causal and Exposure Investigation

* `day08_causal_assessment.csv`
* `day09_campaign_counts.csv`
* `day09_campaign_redemption.csv`
* `day10_customer_campaign_counts.csv`
* `day10_campaign_coupon_summary.csv`
* `day10_coupon_campaign_counts.csv`
* `day10_relationship_validation.csv`

### Days 11–13: Treatment and Exposure Assessment

* `day11_treatment_outcome_assessment.csv`
* `day12_treatment_assignment_assessment.csv`
* `day13_customer_exposure_assessment.csv`

## Day 13 Summary

Day 13 focused on customer-level campaign relationships and the evidence required to establish campaign exposure.

The analysis:

* Validated customer, campaign, and coupon identifiers.
* Examined campaign and coupon counts by customer.
* Investigated repeated customer–campaign–coupon combinations.
* Recorded the findings in `day13_customer_exposure_assessment.csv`.

## Interpretation and Limitations

The outputs are intended to support transparent analysis and reproducibility.

* Identifier matching does not prove treatment assignment.
* Campaign membership does not necessarily establish actual exposure.
* Coupon redemption is an observed outcome, not proof that treatment was randomly assigned.
* Descriptive associations should not be interpreted as causal effects without a defensible identification strategy.

## Data Handling

Raw datasets are excluded from GitHub. CSV reports should contain only the analytical outputs needed to document the project, without unnecessarily exposing sensitive or restricted information.

## Maintenance

When adding a new project day:

1. Save the corresponding daily report.
2. Save the generated CSV outputs.
3. Add the new files to this index.
4. Verify that the filenames match the actual files in the repository.
