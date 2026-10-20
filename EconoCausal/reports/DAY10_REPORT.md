# Day 10 Report — Customer-Campaign Relationship Analysis

## Project
EconoCausal — Dynamic Pricing via Double Machine Learning

## Organization
Infotact Solutions

## Objective
Investigate customer participation across campaigns, coupon distribution, and the structural relationships between customers, campaigns, and coupons.

## Tasks Completed

1. Loaded the training, campaign, and customer demographic datasets.
2. Counted the number of campaigns associated with each customer.
3. Analyzed unique coupons and customers per campaign.
4. Investigated how many campaigns each coupon appears in.
5. Validated customer-campaign combinations.
6. Checked duplicate customer-campaign-coupon combinations.
7. Validated the uniqueness and completeness of training identifiers.
8. Exported the analysis results to CSV files.

## Output Files

- `day10_customer_campaign_counts.csv`
- `day10_campaign_coupon_summary.csv`
- `day10_coupon_campaign_counts.csv`
- `day10_relationship_validation.csv`
- `DAY10_REPORT.md`
- `../notebooks/10_customer_campaign_relationships.ipynb`

## Analysis Overview

### Customer-Campaign Relationships
Examined the number of campaigns, coupons, and training records associated with each customer.

### Campaign-Coupon Relationships
Investigated the number of unique coupons and customers represented in each campaign.

### Coupon-Campaign Relationships
Checked whether coupons appear in multiple campaigns in the training records.

### Relationship Validation
Investigated duplicate customer-campaign combinations, duplicate customer-campaign-coupon combinations, and training identifier uniqueness.

## Key Observations

- Customers may appear in multiple campaign-related training records.
- Campaigns may contain different numbers of customers and coupons.
- Coupon identifiers may be associated with more than one campaign in the observed records.
- Duplicate customer-campaign combinations do not automatically indicate data errors.
- Identifier uniqueness and relationship cardinality must be considered before joining or modeling datasets.

## Causal Analysis Considerations

These analyses describe relationships in the available training records. They do not establish that customers received every associated campaign or that campaign exposure was randomly assigned.

Before estimating a causal effect, the project must establish:

1. A clearly defined treatment or exposure.
2. A measurable outcome.
3. Appropriate pre-treatment covariates.
4. A defensible identification strategy.
5. Sufficient information to compare relevant treatment conditions.

Observed differences and associations alone do not demonstrate causal effects.

## Next Steps

- Investigate the meaning and availability of campaign exposure information.
- Assess whether meaningful comparison groups can be defined.
- Review the limitations of the observational data.
- Determine whether the intended causal question is supported by the available variables.

---

**Status:** Customer-campaign relationship analysis completed.