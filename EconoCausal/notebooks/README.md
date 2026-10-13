# EconoCausal Notebooks

This directory contains the Jupyter notebooks used to inspect and validate the project dataset.

## Day 1 — Initial Dataset Inspection

File: `01_data_inspection.ipynb`

- Loaded the available CSV datasets.
- Examined dataset dimensions.
- Summarized missing values and duplicate records.
- Generated the initial dataset summary.

## Day 2 — Data Quality Analysis

File: `02_data_quality_analysis.ipynb`

- Analyzed missing values.
- Examined duplicate records.
- Checked customer demographic coverage.
- Exported data-quality reports.

## Day 3 — Dataset Relationship Validation

File: `03_dataset_relationships.ipynb`

- Validated training-to-campaign relationships.
- Checked coupon identifiers against coupon-item mapping.
- Investigated customer demographic matches.
- Checked training ID uniqueness.
- Exported relationship and training-structure reports.

## Execution Notes

Run the notebooks in order: Day 1, Day 2, then Day 3.

The notebooks expect the source CSV files to be available in the local `data/raw/` directory. Raw datasets are not included in this repository.

## Important Note

Successful identifier matching does not by itself establish a causal relationship. Treatment definitions, outcome variables, and identification assumptions must be assessed before causal modeling.
