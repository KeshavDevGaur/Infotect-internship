# EconoCausal — Jupyter Notebooks

This folder contains the Jupyter notebooks developed during the EconoCausal project.

Each notebook documents a specific stage of the research workflow, from initial dataset exploration to causal research design and transaction data investigation.

## Notebook Organization

Notebooks are organized chronologically according to the project development timeline.

| Day       | Notebook                                                | Description                                                                       |
| --------- | ------------------------------------------------------- | --------------------------------------------------------------------------------- |
| Day 01–15 | Individual daily notebooks                              | Initial project development, dataset exploration, data preparation, and analysis  |
| Day 16    | `16_dataset_documentation_causal_design.ipynb`          | Dataset documentation and preliminary causal research design                      |
| Day 17    | `17_treatment_definition_identification_strategy.ipynb` | Treatment candidates, outcome definition, and causal identification assessment    |
| Day 18    | `18_dataset_documentation_research.ipynb`               | Original dataset documentation research and transaction measurement investigation |

## Day 16 — Dataset Documentation and Causal Design

**Notebook:** `16_dataset_documentation_causal_design.ipynb`

### Objectives

* Understand the original dataset structure.
* Review available campaign and customer information.
* Identify potential causal research questions.
* Examine the feasibility of causal analysis.

### Key Activities

* Dataset documentation.
* Variable investigation.
* Research design assessment.
* Identification of potential limitations.

### Output

`day16_causal_research_design_assessment.csv`

## Day 17 — Treatment Definition and Identification Strategy

**Notebook:** `17_treatment_definition_identification_strategy.ipynb`

### Objectives

* Identify potential treatment variables.
* Investigate treatment assignment.
* Examine possible outcome variables.
* Assess causal identification requirements.

### Key Activities

* Treatment candidate evaluation.
* Treatment and control group investigation.
* Outcome candidate assessment.
* Identification assumption analysis.

### Outputs

* `day17_treatment_candidate_assessment.csv`
* `day17_causal_identification_assessment.csv`
* `day17_causal_research_assessment.csv`

### Key Finding

The available dataset does not yet establish a sufficiently defensible treatment assignment mechanism or actual campaign exposure.

## Day 18 — Dataset Documentation Research

**Notebook:** `18_dataset_documentation_research.ipynb`

### Objectives

* Investigate original dataset documentation.
* Understand transaction variable definitions.
* Examine extreme transaction quantities.
* Investigate Fuel category purchasing patterns.
* Evaluate potential expenditure measurement limitations.

### Key Activities

**1. Original Dataset Research**

* Reviewed the original AmExpert marketing campaign challenge.
* Investigated campaign and coupon characteristics.
* Reviewed relevant published causal marketing research.

**2. Transaction Data Investigation**

* Examined transaction dates and customer identifiers.
* Investigated quantity and selling price.
* Analyzed discount variables.
* Examined missing values and variable distributions.

**3. Extreme Quantity Investigation**

* Identified unusually large transaction quantities.
* Compared quantity distributions across product categories.
* Investigated frequently observed Fuel items.

**4. Fuel Item Analysis**

* Investigated item 49009.
* Compared other frequently observed Fuel items.
* Calculated price-to-quantity ratios.
* Examined consistency across selected items.

### Key Findings

* Fuel and Miscellaneous categories contain unusually large transaction quantities.
* Several frequently observed Fuel items have relatively consistent price-to-quantity ratios.
* Quantity units and transaction measurement conventions require further documentation.
* The current analysis is descriptive and does not establish causal effects.

### Output

`day18_fuel_item_analysis.csv`

## Notebook Guidelines

* Run notebook cells sequentially.
* Keep code organized and reproducible.
* Include explanations for important findings.
* Use clear variable names.
* Document assumptions and limitations.
* Avoid treating descriptive associations as causal effects.
* Export important analytical results into the reports folder.

## Future Notebooks

Upcoming notebooks will focus on:

* Transaction variable documentation.
* Customer-level outcome construction.
* Campaign exposure investigation.
* Treatment assignment feasibility.
* Confounding and overlap assessment.
* Double Machine Learning feasibility.

**Note:** DML estimation should begin only after treatment, outcome, and identification assumptions have been adequately justified.
