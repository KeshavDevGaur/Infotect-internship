# Day 20 Report — Transaction Measurement Verification and Outcome Feasibility

## 1. Objective

The objective of Day 20 was to investigate transaction measurement conventions and assess whether a reliable customer-level expenditure outcome could be constructed for causal analysis.

The analysis focused on quantity, selling price, discount variables, transaction-level expenditure candidates, and customer-level spending patterns.

## 2. Dataset Information

**Dataset:** `customer_transaction_data.csv`

**Additional Dataset:** `item_data.csv`

**Total Transaction Records:** Approximately 1,324,566.

### Variables Investigated

| Variable        | Description                   |
| --------------- | ----------------------------- |
| date            | Transaction date              |
| customer_id     | Customer identifier           |
| item_id         | Product identifier            |
| quantity        | Recorded transaction quantity |
| selling_price   | Recorded selling price        |
| other_discount  | Other discount                |
| coupon_discount | Coupon discount               |

## 3. Work Completed

### A. Transaction Variable Investigation

* Loaded the original transaction dataset.
* Inspected column names and data types.
* Examined transaction variable availability.
* Documented variables requiring further verification.

### B. Selling Price and Quantity Investigation

* Examined frequently observed items.
* Investigated selling price variation.
* Studied the relationship between quantity and selling price.
* Examined individual item transaction patterns.
* Calculated provisional amount-per-quantity measures.

### C. Discount Measurement Investigation

* Analyzed `other_discount` and `coupon_discount`.
* Investigated negative, zero, and positive values.
* Examined discount patterns across products.
* Compared recorded selling prices with discount-adjusted amounts.
* Investigated negative and zero adjusted amounts.

### D. Product Category Investigation

* Combined transaction data with item metadata.
* Examined transaction patterns across product categories.
* Compared quantity and selling price relationships.
* Investigated adjusted expenditure patterns across categories.
* Examined negative adjusted amounts by category.

### E. Customer-Level Analysis

* Aggregated transaction records by customer.
* Calculated total recorded selling prices.
* Calculated provisional adjusted amounts.
* Investigated customer-level discount impact.
* Compared customers with and without recorded coupon discounts.

### F. Outcome Feasibility Assessment

* Evaluated customer-level aggregation feasibility.
* Examined expenditure measurement limitations.
* Reviewed the availability of transaction and discount variables.
* Assessed whether the available measures were ready for causal analysis.
* Documented the final research recommendation.

## 4. Expenditure Measurement Candidates

Two preliminary expenditure candidates were investigated.

### Candidate A

`selling_price`

This represents the recorded selling price variable.

### Candidate B

`selling_price + other_discount + coupon_discount`

This represents a provisional discount-adjusted amount, assuming the discount columns are monetary deductions.

Neither candidate has been independently verified as the actual customer expenditure measure.

## 5. Important Findings

1. Customer-level transaction aggregation is technically possible.
2. Selling price and discount variables are available.
3. Transaction quantities show different patterns across product categories.
4. Discount-adjusted amounts can be calculated mathematically.
5. Discount patterns vary across products and customers.
6. Observed coupon discounts do not establish actual campaign exposure.
7. Transaction measurement conventions require further documentation.

## 6. Outcome Feasibility Decision

**Preliminary Decision: PARTIALLY FEASIBLE**

Customer-level spending candidates can be constructed using the available transaction data.

However, the exact measurement conventions of quantity, selling price, and discounts have not been sufficiently verified.

Therefore, neither expenditure candidate should yet be treated as a validated causal outcome.

## 7. Research Limitations

* Exact quantity measurement units remain uncertain.
* Selling price may require further interpretation.
* Discount calculation conventions need verification.
* Transaction-level calculations do not automatically represent actual expenditure.
* Customer-level spending is currently descriptive.
* Actual campaign exposure remains unresolved.
* Treatment assignment mechanism remains unresolved.
* Causal identification assumptions require further investigation.

## 8. Research Recommendation

Further investigate the original dataset documentation and validate transaction measurement conventions.

Before applying Double Machine Learning, the project must establish:

1. A clearly defined treatment.
2. A defensible treatment assignment mechanism.
3. A properly measured outcome.
4. Relevant pre-treatment confounders.
5. Appropriate causal identification assumptions.

DML estimation should not begin until these requirements are sufficiently justified.

## 9. Conclusion

Day 20 established that customer-level expenditure analysis is technically possible, but a scientifically validated expenditure outcome has not yet been established.

The project has completed its initial 20-day research plan and established a foundation for the next phase of causal identification and DML feasibility assessment.

## 10. Next Steps

The next research phase will focus on:

* Original transaction variable documentation.
* Customer-level outcome validation.
* Actual campaign exposure investigation.
* Treatment assignment mechanism.
* Confounding variable identification.
* Treatment and control group overlap.
* Causal identification strategy.
* Double Machine Learning feasibility.
