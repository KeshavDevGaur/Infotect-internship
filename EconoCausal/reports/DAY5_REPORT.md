# Day 5 Report — Customer and Coupon Analysis

## Project
EconoCausal — Dynamic Pricing via Double Machine Learning

## Objective
Analyze customer demographics, coupon-item relationships, product categories, and observed coupon redemption patterns.

## Tasks Completed

1. Loaded customer demographics, coupon-item mapping, item information, and training datasets.
2. Analyzed customer age ranges, marital status, and income brackets.
3. Investigated missing demographic values.
4. Visualized customer demographic distributions.
5. Analyzed product categories and brand types.
6. Examined the number of items associated with each coupon.
7. Connected customer demographics with training redemption records.
8. Calculated observed redemption rates by age group.
9. Calculated observed redemption rates by marital status.
10. Calculated observed redemption rates by income bracket.
11. Visualized redemption rates by age group.
12. Exported analysis results to CSV files.

## Reports Generated

- `day05_age_redemption.csv`
- `day05_marital_redemption.csv`
- `day05_income_redemption.csv`
- `day05_coupon_item_counts.csv`
- `day05_category_counts.csv`

## Notebook

`notebooks/05_customer_coupon_analysis.ipynb`

## Key Observations

- Customer demographic information varies across age groups, marital statuses, and income brackets.
- Some demographic fields contain missing values.
- Coupons can be associated with multiple items.
- Product categories and brand types provide information about the available product catalog.
- Observed redemption rates may differ across customer demographic groups.

## Important Limitations

The analysis identifies observational patterns and does not establish causal relationships.

Missing demographic information should be handled carefully. Differences in redemption rates should also be interpreted alongside group sizes.

The presence of transaction discount values does not automatically establish which treatment was assigned to every customer.

## Next Steps

- Investigate transaction behavior and discount-related variables.
- Examine the relationships among campaigns, coupons, customers, and transactions.
- Assess whether the available data supports credible causal-effect estimation.

---

**Status:** Day 5 analysis and documentation in progress.