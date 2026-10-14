# Day 4 Report — Target Variable Analysis

## Project
EconoCausal — Dynamic Pricing via Double Machine Learning

## Objective
Analyze the target variable `redemption_status` and investigate redemption patterns across campaigns and campaign types.

## Tasks Completed
1. Analyzed the distribution of the target variable.
2. Visualized redemption and non-redemption counts.
3. Calculated redemption rates for individual campaigns.
4. Compared redemption rates across campaign types.
5. Identified the top 10 campaigns by redemption rate.
6. Created visualizations to compare campaign performance.
7. Exported analysis results to CSV files.

## Reports Generated
- `day04_campaign_redemption.csv`
- `day04_campaign_type_analysis.csv`
- `day04_top_campaigns.csv`

## Key Findings
- The target variable is `redemption_status`.
- Redemption rates vary across campaigns.
- Campaign-type performance was compared using redemption rates.
- The top 10 campaigns were identified based on their observed redemption rates.

## Important Observation
The dataset is highly imbalanced, with substantially more non-redemption records than redemption records. Therefore, future predictive modeling should not rely on accuracy alone.

Observed redemption rates describe associations in the dataset and do not establish the causal effect of a discount or campaign.

## Next Steps
- Investigate customer and coupon characteristics.
- Explore transaction behavior and discount-related variables.
- Assess whether the available data supports causal-effect estimation.