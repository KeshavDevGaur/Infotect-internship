# EconoCausal — Notebook Documentation

This directory contains the Jupyter notebooks used for dataset exploration, data quality analysis, customer and campaign investigation, and preliminary causal research design.

## Notebook Index

| Notebook                                       | Description                                                 |
| ---------------------------------------------- | ----------------------------------------------------------- |
| `01_data_inspection.ipynb`                     | Initial dataset inspection                                  |
| `02_data_quality_analysis.ipynb`               | Missing values and duplicate analysis                       |
| `03_dataset_relationships.ipynb`               | Dataset relationship validation                             |
| `04_target_analysis.ipynb`                     | Target and campaign redemption analysis                     |
| `05_customer_coupon_analysis.ipynb`            | Customer demographics and coupon relationships              |
| `06_transaction_discount_analysis.ipynb`       | Transaction and discount analysis                           |
| `07_dataset_integration.ipynb`                 | Dataset integration and causal variable exploration         |
| `08_treatment_outcome_analysis.ipynb`          | Preliminary treatment and outcome investigation             |
| `09_campaign_exposure_analysis.ipynb`          | Campaign-level exposure investigation                       |
| `10_customer_campaign_relationships.ipynb`     | Customer-campaign relationship analysis                     |
| `11_treatment_outcome_definition.ipynb`        | Treatment and outcome assessment                            |
| `12_treatment_assignment_analysis.ipynb`       | Treatment-assignment investigation                          |
| `13_customer_exposure_analysis.ipynb`          | Customer-level relationship and exposure assessment         |
| `14_causal_identification_feasibility.ipynb`   | Causal identification feasibility assessment                |
| `15_treatment_assignment_evidence.ipynb`       | Treatment-assignment evidence investigation                 |
| `16_dataset_documentation_causal_design.ipynb` | Dataset documentation and causal research design assessment |

## Day 16 Summary

Day 16 examined campaign metadata and evaluated whether the available data supports a defensible causal research design.

### Tasks Performed

* Inspected campaign metadata and training data.
* Examined campaign types X and Y.
* Compared observed redemption patterns across campaign types.
* Documented questions about customer eligibility, assignment, and exposure.
* Created a structured causal research-design assessment.

## Important Interpretation Notes

* Campaign types are descriptive characteristics until their meanings are verified.
* Campaign membership does not independently establish actual customer exposure.
* `redemption_status` is an observed outcome, not proof of treatment assignment.
* Differences in redemption rates do not automatically establish causal effects.
* Double Machine Learning requires a defensible causal identification strategy.

## Execution Instructions

1. Open JupyterLab.
2. Navigate to this directory.
3. Open the required notebook.
4. Run the cells in order.
5. Ensure the required datasets are available in `../data/raw/`.

Raw datasets are excluded from GitHub and must be obtained separately.

## Reproducibility

The notebooks document the analysis workflow, findings, and limitations. Results should be interpreted according to the available evidence and the assumptions stated in each notebook.

*Verify that each notebook listed above exists before treating this index as a complete inventory.*
