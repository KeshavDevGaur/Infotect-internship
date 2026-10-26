# Day 14 Report — Causal Identification Feasibility

## Project

**EconoCausal — Dynamic Pricing via Double Machine Learning**

## Objective

Assess whether the available AmExpert 2019 Marketing Campaign dataset provides sufficient evidence to define a treatment, identify an outcome, and establish a defensible causal identification strategy.

## Work Completed

* Loaded the training, campaign, customer demographic, and transaction datasets.
* Inspected dataset structures, columns, and sample records.
* Investigated candidate treatment and outcome variables.
* Examined customer demographics and transaction variables as potential covariates.
* Investigated the availability of campaign and transaction dates.
* Documented unresolved questions about treatment assignment and causal identification.
* Generated a structured causal identification feasibility assessment.

## Key Findings

### 1. Candidate Outcome

The `redemption_status` variable is a candidate outcome representing observed coupon redemption. Its suitability depends on the precise causal question being investigated.

### 2. Treatment Definition

A verified treatment variable and treatment-assignment mechanism have not yet been established. Campaign identifiers and campaign characteristics do not independently demonstrate which customers received a particular intervention.

### 3. Potential Confounders

Customer demographic and historical behavioral variables may provide useful covariates. Their timing, relevance, and relationship to treatment assignment and the outcome must be assessed before inclusion in a causal model.

### 4. Temporal Ordering

Campaign dates and transaction dates need to be interpreted and aligned to establish whether candidate covariates were measured before treatment.

### 5. Causal Identification

The current investigation has not established the assumptions or assignment mechanism required to identify a causal effect reliably.

### 6. Double Machine Learning Readiness

Causal effect estimation should not proceed until the treatment, outcome, identification strategy, and appropriate pre-treatment covariates are justified.

## Output File

* `day14_causal_identification_assessment.csv`

## Limitations

This is a preliminary feasibility assessment. The findings do not prove that causal analysis is impossible; they identify the evidence and assumptions that still require investigation.

Observed associations, identifier matches, and coupon redemption alone cannot establish a causal effect.

## Conclusion

Day 14 focused on evaluating the feasibility of causal identification. The analysis identified a candidate outcome and potential covariates while documenting unresolved questions about treatment assignment, exposure, temporal ordering, and causal assumptions.

Further investigation is required before applying Double Machine Learning to estimate causal effects.

## Next Steps

* Investigate available documentation about campaign eligibility, assignment, delivery, and exposure.
* Define a precise causal question and candidate treatment.
* Verify the timing of potential pre-treatment covariates.
* Assess whether the available data supports a defensible identification strategy.
