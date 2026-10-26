# EconoCausal — Reports and Analysis Outputs

This directory contains daily project reports and CSV files generated during the EconoCausal project.

The reports document data exploration, data quality checks, customer and campaign relationships, treatment assessment, and preliminary causal identification analysis.

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
| `DAY14_REPORT.md` | Causal identification feasibility assessment        |

## Analysis Output Files

The following index describes the expected analytical outputs. Verify that each file exists before treating this list as a complete inventory.

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

### Days 11–14: Treatment and Causal Identification

* `day11_treatment_outcome_assessment.csv`
* `day12_treatment_assignment_assessment.csv`
* `day13_customer_exposure_assessment.csv`
* `day14_causal_identification_assessment.csv`

## Day 14 Summary

Day 14 evaluated whether the available datasets provide sufficient evidence for a defensible causal identification strategy.

The analysis:

* Inspected candidate treatment and outcome variables.
* Examined potential confounders and variable timing.
* Investigated campaign and transaction date information.
* Documented unresolved questions about treatment assignment.
* Generated `day14_causal_identification_assessment.csv`.

## Interpretation and Limitations

These reports document exploratory findings and the current state of the project.

* Identifier matches do not establish treatment assignment.
* Campaign associations do not necessarily prove actual customer exposure.
* Coupon redemption is an observed outcome, not proof of randomized treatment.
* Candidate covariates require timing and relevance checks.
* A credible causal estimate requires a clearly defined treatment, an appropriate outcome, and a defensible identification strategy.

## Data Handling

Raw datasets are excluded from GitHub. Reports should contain only the analytical outputs necessary to document the project and should not unnecessarily expose sensitive or restricted information.

## Maintenance

When adding a new project day:

1. Save the corresponding daily report.
2. Save the generated CSV outputs.
3. Update this index.
4. Verify filenames and paths.
5. Confirm that the README accurately reflects the files uploaded to GitHub.
