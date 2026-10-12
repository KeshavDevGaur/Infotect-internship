# Day 2 Report — EconoCausal

## Objective
Analyze dataset quality and investigate relationships between datasets.

## Completed Tasks
- Loaded all eight CSV datasets.
- Identified missing values in customer demographics.
- Detected 2,916 exact duplicate rows in customer transaction data.
- Inspected column names and data types.
- Analyzed redemption-status distribution.
- Checked campaign, coupon, and customer ID coverage.

## Key Findings
- Training records: 78,369.
- Redemption status 0: 77,640 records (99.07%).
- Redemption status 1: 729 records (0.93%).
- All training campaign IDs matched campaign_data.
- All training coupon IDs matched coupon_item_mapping.
- 43,661 training records matched customer demographics.
- 34,708 training records did not match customer demographics.
- 2,916 exact duplicate transaction rows require further investigation.

## Next Steps
- Investigate duplicate transactions.
- Examine relationships between transactions, campaigns, and coupons.
- Determine whether the dataset supports defensible causal estimation.
