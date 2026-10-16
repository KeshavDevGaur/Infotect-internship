# EconoCausal — Jupyter Notebooks

This folder contains the Jupyter notebooks used for dataset inspection, data quality analysis, relationship validation, target analysis, customer-coupon analysis, and transaction-discount analysis.

## Notebook Index

| Notebook | Description | Status |
|---|---|---|
| `01_data_inspection.ipynb` | Loads datasets and examines their dimensions, columns, and structure. | Completed |
| `02_data_quality_analysis.ipynb` | Investigates missing values, duplicate records, and data quality issues. | Completed |
| `03_dataset_relationships.ipynb` | Validates dataset relationships and examines training data structure. | Completed |
| `04_target_analysis.ipynb` | Analyzes redemption patterns, campaign performance, and campaign-type redemption rates. | Completed |
| `05_customer_coupon_analysis.ipynb` | Analyzes customer demographics, coupon-item mappings, product categories, and observed redemption rates. | Completed |
| `06_transaction_discount_analysis.ipynb` | Examines transaction records, selling prices, discount distributions, duplicate rows, and correlations. | Completed |

## Day 6 Analysis

The sixth notebook focuses on transaction and discount data.

The analysis includes:

- Transaction columns and data types.
- Descriptive statistics for numerical variables.
- Selling prices, quantities, and discount values.
- Missing-value analysis.
- Customer transaction activity.
- Exact duplicate transaction checks.
- Coupon discount and other discount distributions.
- Correlations between numerical transaction variables.
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
4. Ensure all required input files are available.
5. Review the generated outputs in the `reports/` directory.

Original dataset files are maintained locally and are not uploaded to GitHub.

## Important Considerations

- Correlation does not establish causation.
- Duplicate transaction rows should not automatically be removed.
- Transaction-level discounts do not necessarily identify the treatment assigned to every customer.
- Causal analysis requires a defensible treatment definition, outcome, covariates, and identification assumptions.

## Upcoming Work

- Investigate relationships between transactions, coupons, campaigns, and redemption outcomes.
- Examine whether a suitable treatment variable can be defined.
- Assess the feasibility of causal effect estimation.
