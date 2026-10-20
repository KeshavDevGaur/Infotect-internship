# EconoCausal — Jupyter Notebooks

This directory contains the Jupyter notebooks developed for the **EconoCausal — Dynamic Pricing via Double Machine Learning** internship project at Infotact Solutions.

The notebooks document dataset inspection, data quality analysis, campaign performance, customer behavior, transaction discounts, dataset integration, and preliminary causal feasibility investigations.

## 📚 Notebook Index

| Day | Notebook | Description | Status |
|---|---|---|---|
| 1 | `01_data_inspection.ipynb` | Dataset inspection, dimensions, columns, and summary statistics | Completed |
| 2 | `02_data_quality_analysis.ipynb` | Missing-value analysis and duplicate detection | Completed |
| 3 | `03_dataset_relationships.ipynb` | Join keys, dataset relationships, and unmatched records | Completed |
| 4 | `04_target_analysis.ipynb` | Redemption distribution and campaign-level analysis | Completed |
| 5 | `05_customer_coupon_analysis.ipynb` | Customer demographics, coupon-item mappings, and category analysis | Completed |
| 6 | `06_transaction_discount_analysis.ipynb` | Transaction patterns, discount variables, missing values, and duplicates | Completed |
| 7 | `07_dataset_integration.ipynb` | Dataset integration, merge validation, and causal-variable investigation | Completed |
| 8 | `08_treatment_outcome_analysis.ipynb` | Preliminary treatment and outcome assessment | Completed |
| 9 | `09_campaign_exposure_analysis.ipynb` | Campaign distribution, redemption rates, and exposure investigation | Completed |
| 10 | `10_customer_campaign_relationships.ipynb` | Customer-campaign relationships, coupon distribution, and relationship validation | Completed |

## 🔍 Notebook Details

### Day 1 — Dataset Inspection

**Notebook:** `01_data_inspection.ipynb`

**Objectives:**
- Load and inspect the available datasets.
- Examine dataset dimensions and column names.
- Review basic dataset information.
- Generate an initial dataset summary.

**Output:**
- `day01_dataset_summary.csv`

### Day 2 — Data Quality Analysis

**Notebook:** `02_data_quality_analysis.ipynb`

**Objectives:**
- Identify missing values.
- Investigate duplicate records.
- Review data-quality issues.
- Generate data-quality summaries.

**Outputs:**
- `day02_missing_values.csv`
- `day02_duplicate_analysis.csv`

### Day 3 — Dataset Relationship Validation

**Notebook:** `03_dataset_relationships.ipynb`

**Objectives:**
- Inspect potential join keys.
- Validate relationships between datasets.
- Investigate unmatched records.
- Examine training dataset structure.

**Outputs:**
- `day03_relationship_validation.csv`
- `day03_training_structure.csv`

### Day 4 — Target and Campaign Analysis

**Notebook:** `04_target_analysis.ipynb`

**Objectives:**
- Analyze the distribution of `redemption_status`.
- Calculate campaign-level redemption statistics.
- Compare campaign types.
- Examine campaigns with higher observed redemption rates.

**Outputs:**
- `day04_campaign_redemption.csv`
- `day04_campaign_type_analysis.csv`
- `day04_top_campaigns.csv`

### Day 5 — Customer and Coupon Analysis

**Notebook:** `05_customer_coupon_analysis.ipynb`

**Objectives:**
- Explore customer demographic characteristics.
- Investigate redemption patterns across customer groups.
- Examine age, marital status, and income-related patterns.
- Analyze coupon-item mappings and item categories.

**Outputs:**
- `day05_age_redemption.csv`
- `day05_marital_redemption.csv`
- `day05_income_redemption.csv`
- `day05_coupon_item_counts.csv`
- `day05_category_counts.csv`

### Day 6 — Transaction and Discount Analysis

**Notebook:** `06_transaction_discount_analysis.ipynb`

**Objectives:**
- Inspect historical transaction records.
- Investigate transaction discount variables.
- Examine missing values and duplicate records.
- Explore discount distributions and correlations.
- Document limitations in interpreting transaction data.

**Outputs:**
- `day06_transaction_summary.csv`
- `day06_missing_values.csv`
- `day06_duplicate_analysis.csv`
- `day06_discount_correlation.csv`

### Day 7 — Dataset Integration

**Notebook:** `07_dataset_integration.ipynb`

**Objectives:**
- Integrate training records with campaign information.
- Integrate customer demographics with training records.
- Connect coupon-item mappings with item information.
- Connect transaction records with customer demographics.
- Validate merge relationships and row preservation.
- Investigate potential causal variables.

**Outputs:**
- `day07_integration_summary.csv`
- `day07_causal_variable_summary.csv`

### Day 8 — Treatment and Outcome Assessment

**Notebook:** `08_treatment_outcome_analysis.ipynb`

**Objectives:**
- Inspect potential treatment and outcome variables.
- Investigate discount-related columns.
- Examine the distribution of the redemption outcome.
- Inspect campaign information.
- Prepare a preliminary causal-variable assessment.
- Document uncertainties concerning treatment assignment.

**Output:**
- `day08_causal_assessment.csv`

### Day 9 — Campaign Exposure Analysis

**Notebook:** `09_campaign_exposure_analysis.ipynb`

**Objectives:**
- Analyze training record counts by campaign.
- Count unique coupons and customers per campaign.
- Calculate campaign-level redemption counts and rates.
- Inspect campaign and training dataset columns.
- Investigate customer demographic coverage.
- Assess whether campaign exposure can be established from the available records.

**Outputs:**
- `day09_campaign_counts.csv`
- `day09_campaign_redemption.csv`

### Day 10 — Customer-Campaign Relationship Analysis

**Notebook:** `10_customer_campaign_relationships.ipynb`

**Objectives:**
- Analyze the number of campaigns associated with each customer.
- Examine coupon distribution across campaigns.
- Investigate how many campaigns each coupon appears in.
- Validate customer-campaign combinations.
- Check duplicate customer-campaign-coupon combinations.
- Validate training identifier uniqueness.
- Document limitations relevant to causal analysis.

**Outputs:**
- `day10_customer_campaign_counts.csv`
- `day10_campaign_coupon_summary.csv`
- `day10_coupon_campaign_counts.csv`
- `day10_relationship_validation.csv`

## 📊 Topics Covered

### Data Inspection and Quality
- Dataset dimensions and column inspection
- Missing-value analysis
- Duplicate detection
- Identifier uniqueness checks
- Data-quality assessment

### Exploratory Data Analysis
- Target distribution
- Campaign redemption patterns
- Customer demographic analysis
- Coupon-item mapping analysis
- Transaction and discount exploration

### Dataset Relationships
- Join-key validation
- Campaign and customer relationships
- Coupon distribution across campaigns
- Dataset integration
- Merge validation and row preservation

### Causal Analysis Preparation
- Preliminary treatment and outcome identification
- Investigation of campaign exposure
- Examination of potential covariates
- Assessment of observational data limitations
- Preliminary evaluation of causal feasibility

## 📁 Outputs and Reports

Analysis summaries and daily reports are stored in the `../reports/` directory.

The reports directory contains:
- Daily Markdown reports
- CSV summaries generated during analysis
- Data-quality results
- Campaign and customer analysis outputs
- Preliminary causal assessment results

## ⚠️ Important Causal Analysis Considerations

The notebooks investigate whether the available data can support a defensible causal analysis.

The observed `redemption_status` variable records coupon redemption in the training dataset. However, recorded transaction discounts have not been established as treatment assignments for all customers.

Campaign identifiers and redemption-rate differences alone do not prove randomized assignment, customer exposure, or causal effects.

Before applying Double Machine Learning, the project must establish:
1. A clearly defined treatment or intervention.
2. A measurable outcome.
3. Appropriate pre-treatment covariates.
4. Defensible identification assumptions.
5. Sufficient data to compare relevant treatment conditions.

## 🛠️ Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- JupyterLab

## 📌 Project Information

- **Project:** EconoCausal — Dynamic Pricing via Double Machine Learning
- **Organization:** Infotact Solutions
- **Domain:** Data Science and Causal Inference
- **Progress:** Days 1–10 completed

---

*These notebooks emphasize reproducible analysis, data validation, transparent assumptions, and responsible interpretation of results.*
