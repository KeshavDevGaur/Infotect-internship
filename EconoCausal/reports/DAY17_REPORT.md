# Day 17 Report — Treatment Definition and Causal Identification Strategy

## Project

EconoCausal — Dynamic Pricing via Double Machine Learning

## Objective

To investigate candidate treatment and outcome variables, assess potential confounding factors, and evaluate possible causal identification strategies.

## Work Completed

1. Loaded the training, campaign metadata, and customer demographic datasets.
2. Inspected candidate treatment and outcome variables.
3. Evaluated campaign type, campaign identifiers, and redemption status.
4. Examined potential customer and campaign covariates.
5. Evaluated randomized experiments, observational adjustment, difference-in-differences, and instrumental variables.
6. Documented findings, limitations, and additional evidence required.
7. Generated three assessment CSV files.

## Key Findings

* The meanings of campaign types X and Y remain unverified.
* The treatment assignment mechanism and actual customer exposure have not been established.
* `redemption_status` is a candidate outcome whose interpretation requires confirmation.
* Customer demographic variables may be relevant covariates, but their suitability for causal adjustment requires further assessment.
* The available evidence does not establish that the assumptions of any evaluated identification strategy are satisfied.
* A defensible DML model cannot yet be specified.

## Files Created

* `17_treatment_definition_identification_strategy.ipynb`
* `day17_treatment_candidate_assessment.csv`
* `day17_causal_identification_assessment.csv`
* `day17_causal_research_assessment.csv`

## Limitations

This analysis is exploratory. It does not establish a causal effect, randomization, or actual campaign exposure. The original assignment mechanism and supporting
