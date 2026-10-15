# EconoCausal — Jupyter Notebooks

This folder contains the Jupyter notebooks used for dataset inspection, data quality analysis, relationship validation, target analysis, and customer-coupon analysis.

## Notebook Index

| Notebook | Description | Status |
|---|---|---|
| `01_data_inspection.ipynb` | Loads datasets and examines their dimensions, columns, and structure. | Completed |
| `02_data_quality_analysis.ipynb` | Investigates missing values, duplicate records, and data quality issues. | Completed |
| `03_dataset_relationships.ipynb` | Validates dataset relationships and examines training data structure. | Completed |
| `04_target_analysis.ipynb` | Analyzes redemption patterns, campaign performance, and campaign-type redemption rates. | Completed |
| `05_customer_coupon_analysis.ipynb` | Analyzes customer demographics, coupon-item mappings, product categories, and observed redemption rates across demographic groups. | Completed |

## Day 5 Analysis

The fifth notebook investigates customer demographics and coupon characteristics.

The analysis includes:

- Customer age range distribution.
- Marital status and income bracket distribution.
- Missing demographic values.
- Product category and brand type analysis.
- Number of items associated with each coupon.
- Redemption rates by age group.
- Redemption rates by marital status.
- Redemption rates by income bracket.
- Exporting analysis results to CSV files.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- JupyterLab

## How to Run the Notebooks

1. Open the project in JupyterLab.
2. Place the original CSV files in the local `data/raw/` directory.
3. Run the notebooks in numerical order.
4. Ensure the required input files are available.
5. Review the generated outputs in the `reports/` directory.

The original dataset files are excluded from GitHub.

## Important Considerations

The demographic analysis describes observed associations and does not establish causal relationships. Missing demographic values and differences in group sizes should be considered when interpreting redemption rates.

## Upcoming Work

- Investigate transaction behavior and discount-related variables.
- Examine campaign, coupon, customer, and transaction relationships.
- Assess whether the available data supports causal effect estimation.
