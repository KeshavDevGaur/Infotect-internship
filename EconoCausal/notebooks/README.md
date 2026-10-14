
---


# EconoCausal — Jupyter Notebooks

This folder contains the Jupyter notebooks used for dataset inspection, data quality analysis, relationship validation, and target variable analysis.

## Notebook Index

| Notebook | Description | Status |
|---|---|---|
| `01_data_inspection.ipynb` | Loads datasets and examines their dimensions, columns, and structure. | Completed |
| `02_data_quality_analysis.ipynb` | Investigates missing values, duplicate records, and data quality issues. | Completed |
| `03_dataset_relationships.ipynb` | Validates dataset relationships and examines training data structure. | Completed |
| `04_target_analysis.ipynb` | Analyzes redemption patterns, campaign performance, and campaign-type redemption rates. | Completed |

## Day 4 Analysis

The fourth notebook focuses on the target variable:

`redemption_status`

The analysis includes:

- Target variable distribution.
- Redemption and non-redemption counts.
- Campaign-level redemption rates.
- Comparison of redemption rates across campaign types.
- Identification of the top 10 campaigns by observed redemption rate.
- Campaign performance visualization.
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

The original dataset files are excluded from GitHub.

## Upcoming Work

- Investigate customer and coupon characteristics.
- Explore transaction behavior.
- Analyze discount-related variables.
- Assess the feasibility of causal effect estimation.
