# EconoCausal — Notebook Documentation

This directory contains the Jupyter notebooks used for data exploration, data quality checks, customer and campaign analysis, and preliminary causal inference investigation.

## Notebook Index

| Notebook                                   | Description                                                                                         |
| ------------------------------------------ | --------------------------------------------------------------------------------------------------- |
| `01_data_inspection.ipynb`                 | Initial dataset inspection and structural overview                                                  |
| `02_data_quality_analysis.ipynb`           | Missing values, duplicate records, and data quality                                                 |
| `03_dataset_relationships.ipynb`           | Validation of relationships between datasets                                                        |
| `04_target_analysis.ipynb`                 | Redemption outcome and campaign analysis                                                            |
| `05_customer_coupon_analysis.ipynb`        | Customer demographics and coupon relationships                                                      |
| `06_transaction_discount_analysis.ipynb`   | Transaction patterns and discount-related analysis                                                  |
| `07_dataset_integration.ipynb`             | Integration of relevant datasets                                                                    |
| `08_treatment_outcome_analysis.ipynb`      | Preliminary treatment and outcome investigation                                                     |
| `09_campaign_exposure_analysis.ipynb`      | Campaign-level exposure investigation                                                               |
| `10_customer_campaign_relationships.ipynb` | Customer-campaign relationships                                                                     |
| `11_treatment_outcome_definition.ipynb`    | Assessment of potential treatment and outcome definitions                                           |
| `12_treatment_assignment_analysis.ipynb`   | Investigation of treatment assignment evidence                                                      |
| `13_customer_exposure_analysis.ipynb`      | Customer-level relationships, identifier validation, repeated combinations, and exposure assessment |

## Day 13 Summary

The Day 13 notebook investigates whether the available datasets establish customer-level campaign exposure.

Tasks include:

* Loading the relevant datasets.
* Validating customer, campaign, and coupon identifiers.
* Summarizing campaign and coupon relationships for each customer.
* Checking repeated customer–campaign–coupon combinations.
* Recording the evidence and limitations in a structured assessment.

## Important Interpretation Note

Identifier matches and observed customer-campaign relationships do not independently prove treatment assignment or actual exposure.

The analyses are exploratory and descriptive. A defensible causal analysis requires a clearly defined treatment, a suitable outcome, and a justified identification strategy.

## Execution

1. Open JupyterLab.
2. Navigate to this directory.
3. Open the relevant notebook.
4. Run the cells in order.
5. Confirm that the required local datasets are available in `../data/raw/`.

Raw datasets are excluded from GitHub and must be obtained separately.

## Reproducibility

The notebooks are intended to document the analysis workflow. Outputs and conclusions should be interpreted in light of the data available and the assumptions stated in each notebook.

*Note: Ensure every notebook listed above exists in the repository before publishing this index as a complete inventory.*
