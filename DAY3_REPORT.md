# Day 3 Report — Dataset Relationships

## Project
EconoCausal: Dynamic Pricing via Double Machine Learning

## Objectives
- Validate relationships between the training dataset and supporting datasets.
- Check training, campaign, coupon, and customer identifiers.
- Identify potential data-quality issues.

## Key Findings
- Training records: 78,369
- Unique training IDs: 78,369
- Unique campaigns: 18
- Unique coupons: 866
- Unique customers: 1,428
- Duplicate training IDs: 0
- Training-to-campaign matching: 100%
- Training-to-coupon-mapping matching: 100%
- Training records matching customer demographics: 55.71%
- Training records without demographic matches: 44.29%

## Generated Reports
- day03_relationship_validation.csv
- day03_training_structure.csv

## Conclusion
The training dataset has unique record identifiers. The campaign and coupon identifier checks passed. However, 44.29% of training records lack matching demographic information. This issue must be considered during preprocessing.

## Next Steps
- Investigate customer-level data coverage.
- Examine the target variable and available features.
- Assess whether the dataset contains the treatment and outcome variables needed for causal pricing analysis.