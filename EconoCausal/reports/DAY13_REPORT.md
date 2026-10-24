# Day 13 Report — Customer-Level Treatment and Exposure Investigation

## Project

**EconoCausal — Dynamic Pricing via Double Machine Learning**

## Objective

Investigate the relationships between customers, campaigns, and coupons to assess whether the available datasets establish customer-level campaign exposure.

## Work Completed

* Loaded the training, campaign, customer demographic, coupon mapping, and transaction datasets.
* Inspected relevant columns and sample records.
* Validated customer, campaign, and coupon identifiers against their corresponding datasets.
* Analyzed the number of campaigns, coupons, and training records associated with each customer.
* Checked for repeated customer–campaign–coupon combinations.
* Created a structured customer exposure assessment.

## Key Findings

1. Customer, campaign, and coupon identifiers can be used to investigate relationships across the available datasets.
2. Customer-level campaign and coupon counts describe the structure of the training data.
3. Repeated customer–campaign–coupon combinations require investigation before interpreting them as independent observations.
4. Identifier matches and observed relationships do not establish whether a customer was actually assigned to or exposed to a treatment.
5. The available evidence from these checks is insufficient to verify customer-level treatment assignment.

## Output Files

* `day13_customer_exposure_assessment.csv`

## Limitations

* The analysis does not independently establish treatment assignment or actual campaign exposure.
* Observed coupon redemption is not equivalent to randomized treatment assignment.
* Campaign and coupon relationships may reflect selection effects or other confounding factors.
* Additional documentation or data describing treatment eligibility, assignment, delivery, and exposure may be necessary to support a defensible causal design.

## Conclusion

Day 13 examined customer-level relationships and assessed the evidence for campaign exposure. The analysis provides useful structural information, but verified treatment assignment remains unresolved. This distinction must be addressed before applying Double Machine Learning to estimate causal effects.

## Next Steps

* Review the evidence for treatment assignment and exposure.
* Identify a defensible treatment variable and outcome.
* Define the assumptions required for causal identification before estimating treatment effects.
