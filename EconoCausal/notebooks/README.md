# EconoCausal — Notebook Documentation

This directory contains Jupyter notebooks for data exploration, data quality analysis, customer and campaign investigation, and preliminary causal inference assessment.

## Notebook Index

| Notebook                                     | Description                                         |
| -------------------------------------------- | --------------------------------------------------- |
| `01_data_inspection.ipynb`                   | Initial dataset inspection                          |
| `02_data_quality_analysis.ipynb`             | Missing values and duplicate analysis               |
| `03_dataset_relationships.ipynb`             | Dataset relationship validation                     |
| `04_target_analysis.ipynb`                   | Target and campaign redemption analysis             |
| `05_customer_coupon_analysis.ipynb`          | Customer demographics and coupon relationships      |
| `06_transaction_discount_analysis.ipynb`     | Transaction and discount analysis                   |
| `07_dataset_integration.ipynb`               | Dataset integration and causal variable exploration |
| `08_treatment_outcome_analysis.ipynb`        | Preliminary treatment and outcome investigation     |
| `09_campaign_exposure_analysis.ipynb`        | Campaign-level exposure investigation               |
| `10_customer_campaign_relationships.ipynb`   | Customer-campaign relationship analysis             |
| `11_treatment_outcome_definition.ipynb`      | Treatment and outcome assessment                    |
| `12_treatment_assignment_analysis.ipynb`     | Treatment-assignment investigation                  |
| `13_customer_exposure_analysis.ipynb`        | Customer-level relationship and exposure assessment |
| `14_causal_identification_feasibility.ipynb` | Causal identification feasibility assessment        |
| `15_treatment_assignment_evidence.ipynb`     | Investigation of treatment-assignment evidence      |

## Day 15 Summary

Day 15 investigated whether the available datasets provide evidence of treatment assignment and customer-level campaign exposure.

### Tasks Performed

* Inspected training, campaign, and customer demographic datasets.
* Examined columns potentially related to treatment, eligibility, assignment, delivery, and exposure.
* Investigated campaign types and campaign-level record counts.
* Compared observed redemption rates across campaign types descriptively.
* Documented unresolved questions about treatment definition and customer exposure.
* Created a structured treatment-assignment evidence assessment.

## Important Interpretation Notes

* `redemption_status` is a candidate observed outcome, not proof of treatment assignment.
* `campaign_id` identifies a campaign but does not independently establish customer exposure.
* `campaign_type` is a descriptive characteristic unless the intervention it represents is established.
* Differences in redemption rates are descriptive and should not automatically be interpreted as causal effects.
* Double Machine Learning requires a defensible causal identification strategy.

## Execution Instructions

1. Open JupyterLab.
2. Navigate to this directory.
3. Open the required notebook.
4. Run the cells in order.
5. Ensure the required local datasets are available in `../data/raw/`.

Raw datasets are excluded from GitHub and must be obtained separately.

## Reproducibility

The notebooks document the analysis workflow, findings, and limitations. Interpret results according to the evidence available and the assumptions stated in each notebook.

*Verify that each notebook listed above exists before treating this index as a complete inventory.*
