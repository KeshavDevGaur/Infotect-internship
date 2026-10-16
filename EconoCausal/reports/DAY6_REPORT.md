# Day 6 Report — Transaction and Discount Analysis

## Project
EconoCausal — Dynamic Pricing via Double Machine Learning

## Objective
Analyze transaction data, selling prices, discount variables, customer activity, and data quality to understand the available information for future causal analysis.

## Tasks Completed

1. Loaded the transaction, campaign, and training datasets.
2. Inspected transaction columns and data types.
3. Examined descriptive statistics for selling prices, discounts, and quantities.
4. Investigated missing values in the transaction dataset.
5. Examined customer activity and transaction record counts.
6. Investigated exact duplicate transaction rows.
7. Analyzed coupon discount and other discount distributions.
8. Examined correlations between numerical transaction variables.
9. Created discount distribution visualizations and a correlation heatmap.
10. Exported analysis results to CSV files.

## Reports Generated

- `day06_transaction_summary.csv`
- `day06_missing_values.csv`
- `day06_duplicate_analysis.csv`
- `day06_discount_correlation.csv`

## Notebook

`notebooks/06_transaction_discount_analysis.ipynb`

## Key Observations

- Transaction records contain information about customers, items, selling prices, quantities, and discount values.
- Missing values and duplicate rows were investigated.
- Customer activity was examined using transaction record counts.
- Coupon discounts and other discounts were analyzed separately.
- Correlations between numerical transaction variables were calculated.

## Important Limitations

- Duplicate rows should not automatically be deleted without understanding their meaning.
- Repeated customer-item combinations do not necessarily represent duplicate transactions.
- Correlation does not establish causation.
- Transaction-level discount values do not automatically identify which discount treatment was assigned to every customer.
- Causal analysis requires a defensible treatment definition, outcome, covariates, and identification assumptions.

## Next Steps

- Investigate relationships between transactions, coupons, campaigns, and redemption outcomes.
- Examine the available variables for defining treatment and outcome.
- Assess whether the dataset supports credible causal effect estimation.

---

**Status:** Day 6 transaction and discount analysis completed.