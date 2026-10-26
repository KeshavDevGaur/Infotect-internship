# EconoCausal — Notebook Documentation

This directory contains the Jupyter notebooks used for data exploration, data quality analysis, customer and campaign investigation, and preliminary causal inference assessment.

## Notebook Index

| Notebook                                     | Description                                          |
| -------------------------------------------- | ---------------------------------------------------- |
| `01_data_inspection.ipynb`                   | Initial dataset inspection                           |
| `02_data_quality_analysis.ipynb`             | Missing values and duplicate analysis                |
| `03_dataset_relationships.ipynb`             | Dataset relationship validation                      |
| `04_target_analysis.ipynb`                   | Target and campaign redemption analysis              |
| `05_customer_coupon_analysis.ipynb`          | Customer demographics and coupon relationships       |
| `06_transaction_discount_analysis.ipynb`     | Transaction and discount analysis                    |
| `07_dataset_integration.ipynb`               | Dataset integration and causal variable exploration  |
| `08_treatment_outcome_analysis.ipynb`        | Preliminary treatment and outcome investigation      |
| `09_campaign_exposure_analysis.ipynb`        | Campaign-level exposure investigation                |
| `10_customer_campaign_relationships.ipynb`   | Customer-campaign relationship analysis              |
| `11_treatment_outcome_definition.ipynb`      | Treatment and outcome assessment                     |
| `12_treatment_assignment_analysis.ipynb`     | Treatment assignment investigation                   |
| `13_customer_exposure_analysis.ipynb`        | Customer-level relationships and exposure assessment |
| `14_causal_identification_feasibility.ipynb` | Causal identification feasibility assessment         |

## Day 14 Summary

The Day 14 notebook evaluates whether the available AmExpert 2019 Marketing Campaign datasets provide sufficient evidence to define a treatment and establish a defensible causal identification strategy.

### Tasks Performed

* Loaded and inspected relevant datasets.
* Reviewed candidate treatment and outcome variables.
* Examined potential confounders and variable timing.
* Investigated the availability of campaign and transaction dates.
* Documented unresolved questions about treatment assignment and causal identification.
* Created a structured feasibility assessment.

## Important Interpretation Notes

* `redemption_status` is a candidate outcome, not proof of treatment assignment.
* Campaign identifiers and campaign characteristics do not independently establish actual customer exposure.
* Potential covariates must be evaluated for their timing and relevance.
* Post-treatment variables should not automatically be used as baseline confounders.
* Double Machine Learning does not remove the need for a defensible causal identification strategy.

## Execution Instructions

1. Open JupyterLab.
2. Navigate to this directory.
3. Open the required notebook.
4. Run its cells in order.
5. Confirm that the required datasets are available in `../data/raw/`.

Raw datasets are excluded from GitHub and must be obtained separately.

## Reproducibility

Notebooks document the analysis process and its limitations. Interpret the findings according to the evidence available and the assumptions stated in each notebook.

*Verify that every listed notebook exists in the repository before treating this index as a complete inventory.*
