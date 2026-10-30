# DAY 18 REPORT

## Project: EconoCausal — Dynamic Pricing via Double Machine Learning

### Objective

Investigate unusual transaction quantities, examine Fuel item pricing patterns, and identify potential dataset interpretation issues.

### Work Completed

1. Investigated extreme transaction quantities.
2. Examined Fuel category transactions.
3. Analyzed item 49009 in detail.
4. Calculated price-to-quantity ratios.
5. Compared frequently observed Fuel items.
6. Filtered items with at least 10 transaction records.
7. Exported the comparison results to CSV.

### Key Findings

* Item 49009 has 13,540 transaction records.
* Its average quantity is approximately 10,871.49.
* Quantity and selling price correlation is 0.9538.
* Six Fuel items have at least 10 records.
* Their mean price-to-quantity ratio is approximately 0.086807.
* The ratios are relatively consistent across these six items.

### Output Files

* `day18_fuel_item_analysis.csv`
* `18_dataset_documentation_research.ipynb`

### Limitations

* Exact quantity units are not confirmed.
* The meaning of selling price requires documentation.
* Extreme values should not automatically be treated as errors.
* These descriptive findings do not establish causal treatment effects.

### Conclusion

The investigation identified a distinct transaction pattern among frequently observed Fuel items. Further dataset documentation is required to establish the measurement conventions and interpret these variables correctly.

### Next Steps

Continue investigating dataset documentation, treatment assignment, campaign exposure, and the feasibility of a defensible causal research design.
