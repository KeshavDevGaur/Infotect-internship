# EconoCausal — Reports and Analysis Outputs

This directory contains daily project reports and CSV assessment files generated during the EconoCausal project.

The reports document data exploration, data quality checks, customer and campaign relationships, treatment assessment, and preliminary causal identification investigations.

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
| `DAY12_REPORT.md` | Treatment-assignment assessment                     |
| `DAY13_REPORT.md` | Customer-level treatment and exposure investigation |
| `DAY14_REPORT.md` | Causal identification feasibility assessment        |
| `DAY15_REPORT.md` | Treatment-assignment evidence investigation         |

## Analysis Output Files

The following list describes expected outputs. Verify that each file exists before treating this index as a complete inventory.

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

### Days 11–15: Treatment and Causal Identification

* `day11_treatment_outcome_assessment.csv`
* `day12_treatment_assignment_assessment.csv`
* `day13_customer_exposure_assessment.csv`
* `day14_causal_identification_assessment.csv`
* `day15_treatment_assignment_evidence.csv`

## Day 15 Summary

Day 15 investigated whether the available datasets establish treatment assignment, customer eligibility, and actual campaign exposure.

The analysis:

* Inspected training, campaign, and customer demographic datasets.
* Examined potentially relevant treatment and exposure columns.
* Investigated campaign types and campaign-level record counts.
* Compared redemption rates descriptively across campaign types.
* Documented unresolved questions about treatment assignment.
* Generated `day15_treatment_assignment_evidence.csv`.

## Interpretation and Limitations

* Identifier matches do not establish treatment assignment.
* Campaign membership does not necessarily prove actual customer exposure.
* Coupon redemption is an observed outcome, not proof of randomized treatment.
* Campaign-type differences are descriptive unless a defensible causal comparison is established.
* A credible causal estimate requires a clearly defined treatment, a suitable outcome, and a defensible identification strategy.

## Data Handling

Raw datasets are excluded from GitHub. Reports should contain only the analytical outputs necessary to document the project and should not unnecessarily expose sensitive or restricted information.

## Maintenance

When adding a new project day:

1. Save the corresponding daily report.
2. Save the generated CSV outputs.
3. Update this index.
4. Verify the filenames and paths.
5. Confirm that the README accurately reflects the files uploaded to GitHub.
