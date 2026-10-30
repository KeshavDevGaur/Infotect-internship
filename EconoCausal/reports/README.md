# EconoCausal — Reports and Research Outputs

This folder contains reports, analytical summaries, assessment files, and exported results generated during the EconoCausal project.

The reports document the project's research progress, findings, assumptions, and limitations.

## Folder Contents

### Day 16 — Dataset Documentation and Causal Design

**Report:** `DAY16_REPORT.md`

**Assessment file:**

* `day16_causal_research_design_assessment.csv`

**Work completed:**

* Reviewed dataset structure.
* Investigated available variables.
* Documented potential causal research questions.
* Assessed preliminary causal research feasibility.

**Objective:**

Establish an initial understanding of the dataset and identify requirements for a defensible causal research design.

### Day 17 — Treatment Definition and Identification Strategy

**Report:** `DAY17_REPORT.md`

**Assessment files:**

* `day17_treatment_candidate_assessment.csv`
* `day17_causal_identification_assessment.csv`
* `day17_causal_research_assessment.csv`

**Work completed:**

* Evaluated potential treatment variables.
* Investigated treatment assignment.
* Examined possible outcome variables.
* Assessed causal identification assumptions.
* Documented unresolved research limitations.

**Key finding:**

The available information does not yet establish actual campaign exposure or a reliable treatment assignment mechanism.

### Day 18 — Dataset Documentation Research

**Report:** `DAY18_REPORT.md`

**Assessment file:**

* `day18_fuel_item_analysis.csv`

**Work completed:**

* Investigated extreme transaction quantities.
* Analyzed Fuel category transaction patterns.
* Examined item 49009 and other frequently observed Fuel items.
* Compared price-to-quantity ratios.
* Documented transaction measurement limitations.

**Key finding:**

Six frequently observed Fuel items showed relatively consistent price-to-quantity ratios, with a mean of approximately 0.086807.

**Conclusion:**

The transaction patterns require further documentation before constructing a reliable customer expenditure outcome.

## Output File Descriptions

| File                                          | Description                                |
| --------------------------------------------- | ------------------------------------------ |
| `DAY16_REPORT.md`                             | Day 16 research summary                    |
| `DAY17_REPORT.md`                             | Day 17 research summary                    |
| `DAY18_REPORT.md`                             | Day 18 research summary                    |
| `day16_causal_research_design_assessment.csv` | Preliminary causal research assessment     |
| `day17_treatment_candidate_assessment.csv`    | Evaluation of possible treatment variables |
| `day17_causal_identification_assessment.csv`  | Causal identification assessment           |
| `day17_causal_research_assessment.csv`        | Overall causal research assessment         |
| `day18_fuel_item_analysis.csv`                | Analysis of frequently observed Fuel items |

## Research Principles

All analytical outputs should follow these principles:

1. Maintain reproducibility.
2. Clearly document assumptions.
3. Separate descriptive analysis from causal conclusions.
4. Investigate data quality before model development.
5. Avoid unsupported interpretations of anonymized variables.
6. Preserve the distinction between treatment exposure and coupon redemption.
7. Document limitations alongside findings.

## Upcoming Reports

Future reports may include:

* Transaction variable definition assessment.
* Customer-level outcome construction.
* Campaign exposure assessment.
* Treatment assignment analysis.
* Confounding and overlap assessment.
* DML feasibility assessment.
* Model estimation and robustness analysis.

## Important Note

The presence of an analytical result does not automatically establish a causal relationship.

Causal estimates will be considered only after the treatment, outcome, and identification strategy are adequately justified.
