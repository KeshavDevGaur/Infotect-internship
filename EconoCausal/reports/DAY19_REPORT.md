# Day 19 Report — Transaction Outcome Validation

## 1. Objective

The objective of Day 19 was to investigate transaction-level variables and evaluate whether reliable customer-level expenditure measures could be constructed for causal analysis.

The analysis focused on quantity, selling price, discounts, transaction frequency, and customer-level spending patterns.

## 2. Dataset

**Dataset:** `customer_transaction_data.csv`

**Total Records:** Approximately 1,324,566 transactions.

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

### A. Transaction Data Inspection

* Loaded the transaction dataset.
* Examined column names and data types.
* Checked missing values and duplicate records.
* Investigated transaction date coverage.

### B. Quantity and Selling Price Analysis

* Examined statistical distributions.
* Investigated unusual quantity values.
* Studied the relationship between quantity and selling price.
* Calculated a provisional price-per-quantity ratio.
* Investigated item-level price variation.

### C. Discount Analysis

* Examined `other_discount` and `coupon_discount`.
* Investigated negative, zero, and positive discount values.
* Identified different discount combinations.
* Compared recorded selling price with a discount-adjusted candidate amount.

### D. Customer-Level Analysis

Aggregated transaction records using `customer_id`.

Created the following measures:

* Total transactions.
* Total quantity.
* Total recorded selling price.
* Total adjusted amount.
* Total other discount.
* Total coupon discount.

### E. Customer Spending Investigation

* Examined customer-level spending distributions.
* Identified customers with extreme recorded spending.
* Calculated spending percentiles.
* Investigated spending concentration among the top 10% of customers.
* Examined the relationship between transaction frequency and spending.
* Compared spending across transaction-frequency groups.

### F. Data Validation

* Checked missing customer-level spending values.
* Identified zero and negative values.
* Exported customer-level analysis.
* Reloaded the exported CSV to verify its contents.

## 4. Expenditure Candidates

Two preliminary expenditure candidates were investigated.

**Candidate A:**

`selling_price`

**Candidate B:**

`selling_price + other_discount + coupon_discount`

Candidate B assumes that the discount columns represent monetary reductions from the recorded selling price.

This assumption has not yet been independently verified.

Neither candidate is currently established as the actual customer expenditure measure.

## 5. Important Findings

1. Transaction-level data can be aggregated at customer level.
2. Discount variables contain negative values in the observed dataset.
3. Fuel transactions exhibit unusual quantity patterns.
4. Item-level analysis helps investigate transaction measurement conventions.
5. Customer-level spending measures can be compared descriptively.
6. Transaction frequency and spending can be investigated using customer-level aggregation.
7. The exact definitions of quantity and selling price remain important unresolved questions.

## 6. Research Limitations

* The exact units and meaning of `quantity` require verification.
* The definition of `selling_price` must be established.
* The correct treatment of discount variables remains unconfirmed.
* Extreme transaction quantities should not automatically be treated as errors.
* Customer-level aggregates are descriptive measures.
* Neither expenditure candidate has been validated as a causal outcome.
* Customer-level spending alone does not establish campaign effects.

## 7. Output Files

**Notebook:**

`19_transaction_outcome_validation.ipynb`

**CSV Output:**

`day19_customer_spending_analysis.csv`

The CSV contains customer-level transaction counts, quantity totals, spending candidates, discount totals, and transaction-frequency groups.

## 8. Conclusion

Day 19 established an exploratory customer-level transaction analysis and compared two preliminary expenditure candidates.

The investigation provides a foundation for further outcome validation. However, the exact measurement conventions of transaction quantity, selling price, and discounts must be established before selecting a reliable customer-level expenditure outcome.

Causal modelling and Double Machine Learning estimation should not begin until the outcome definition and causal identification strategy are sufficiently justified.

## 9. Next Steps — Day 20

* Investigate original transaction variable definitions.
* Verify the meaning of selling price and quantity.
* Validate discount calculation conventions.
* Investigate whether customer-level spending can represent a defensible outcome.
* Document the final outcome feasibility assessment.
