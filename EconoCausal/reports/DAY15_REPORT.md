# Day 15 Report — Treatment Assignment Evidence

## Project

**EconoCausal — Dynamic Pricing via Double Machine Learning**

## Objective

Investigate whether the available AmExpert 2019 Marketing Campaign datasets provide sufficient evidence to establish treatment assignment, customer eligibility, and actual campaign exposure.

## Work Completed

* Loaded and inspected the training, campaign, and customer demographic datasets.
* Examined columns that might indicate treatment, eligibility, assignment, or exposure.
* Investigated campaign types and campaign-level record counts.
* Examined customer counts and coupon redemption rates across campaigns.
* Compared observed redemption rates across campaign types descriptively.
* Created a structured treatment-assignment evidence assessment.

## Key Findings

### 1. Treatment Definition

A verified treatment variable has not yet been established by the current investigation.

### 2. Customer Eligibility and Exposure

Campaign membership and identifier relationships do not independently establish whether a customer was eligible for, assigned to, or exposed to a particular intervention.

### 3. Campaign Type

Campaign type is a descriptive campaign characteristic unless the intervention represented by each type is established. Differences between campaign types should not automatically be interpreted as treatment effects.

### 4. Redemption Outcome

The `redemption_status` variable is a candidate observed outcome. Redemption does not independently establish treatment assignment.

### 5. Treated-versus-Control Comparison

A defensible treatment contrast has not yet been established. Further evidence about the campaign-generation process and customer assignment is required.

### 6. Causal Inference Readiness

The available analysis does not yet justify estimating causal effects using Double Machine Learning.

## Output File

* `day15_treatment_assignment_evidence.csv`

## Limitations

This assessment describes the evidence examined so far. It does not establish that treatment-assignment information is unavailable from all possible sources.

The analysis is descriptive and does not demonstrate causal effects.

## Conclusion

Day 15 investigated evidence related to treatment assignment and customer-level campaign exposure. The analysis documented unresolved questions about treatment definition, eligibility, exposure, and the validity of a treated-versus-control comparison.

Before causal estimation, the project requires a clearly defined intervention, a defensible assignment mechanism or identification strategy, an appropriate outcome, and justified assumptions.

## Next Steps

* Review the dataset documentation and available campaign-generation information.
* Investigate whether customer eligibility, assignment, or delivery records are available.
* Define a precise causal question and treatment contrast.
* Determine whether the available evidence supports a defensible causal identification strategy.
