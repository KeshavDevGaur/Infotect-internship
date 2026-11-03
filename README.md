# 📊 EconoCausal

### Customer Coupon Redemption Prediction & Causal Campaign Analysis

**EconoCausal** is a machine learning and data science project designed to analyze customer coupon redemption behaviour, understand promotional campaign performance, and investigate how offers may influence customer purchasing behaviour.

The project combines exploratory data analysis, customer behaviour analysis, feature engineering, machine learning, and causal inference feasibility assessment to develop a foundation for data-driven marketing decisions.

---

## 🎯 Project Objectives

The main objectives of EconoCausal are:

* Analyze customer purchasing and coupon redemption behaviour.
* Understand the relationship between customers, campaigns, coupons, and transactions.
* Identify important factors associated with coupon redemption.
* Develop a machine learning model to predict coupon redemption.
* Investigate whether promotional offers influence customer purchasing behaviour.
* Explore treatment assignment, campaign exposure, and causal identification.
* Develop a Streamlit interface for model deployment.

---

## 💡 Problem Statement

Businesses frequently distribute promotional coupons to increase customer engagement and sales.

However, an important question remains:

**Does providing a promotional offer actually change customer purchasing behaviour, or would customers have purchased anyway?**

Traditional redemption prediction models estimate whether customers are likely to redeem coupons but do not necessarily measure the actual incremental impact of an offer.

EconoCausal addresses this problem through two complementary approaches:

1. **Predictive Analysis:** Predicting customer coupon redemption using machine learning.
2. **Causal Analysis:** Investigating whether available data supports measuring the actual impact of promotional offers.

---

## 📂 Dataset Description

The project uses the **AmExpert 2019 Marketing Campaign dataset**.

The dataset contains information about customers, campaigns, coupons, products, and transactions.

### Main Dataset Files

| Dataset                       | Description                                |
| ----------------------------- | ------------------------------------------ |
| train.csv                     | Training data containing redemption status |
| test_QyjYwdj.csv              | Test dataset                               |
| campaign_data.csv             | Campaign information                       |
| customer_demographics.csv     | Customer demographic information           |
| customer_transaction_data.csv | Customer purchase transactions             |
| coupon_item_mapping.csv       | Coupon-to-item mapping                     |
| item_data.csv                 | Product and item information               |
| sample_submission_Byiv0dS.csv | Sample submission format                   |

### Important Features

* Customer ID
* Campaign ID
* Coupon ID
* Campaign Type
* Age Range
* Marital Status
* Income Bracket
* Family Size
* Purchase Frequency
* Total Spending
* Coupon Discount
* Other Discount
* Campaign Duration
* Redemption Status

**Target Variable:** `redemption_status`

---

## 🛠️ Technology Stack

| Category                | Technologies        |
| ----------------------- | ------------------- |
| Programming Language    | Python              |
| Data Analysis           | Pandas, NumPy       |
| Data Visualization      | Matplotlib, Seaborn |
| Machine Learning        | Scikit-learn        |
| Model Serialization     | Joblib              |
| Development Environment | JupyterLab          |
| Deployment              | Streamlit           |
| Version Control         | Git & GitHub        |

---

## 🔬 Project Workflow

The project was developed through 20 structured analysis notebooks.

### Phase 1: Data Understanding and Exploration

| Day | Notebook                      | Objective                                  |
| --- | ----------------------------- | ------------------------------------------ |
| 01  | Data Inspection               | Understanding datasets and structure       |
| 02  | Data Quality Analysis         | Missing values and duplicate checks        |
| 03  | Dataset Relationships         | Identifying relationships between datasets |
| 04  | Target Analysis               | Understanding redemption status            |
| 05  | Customer Coupon Analysis      | Exploring customer and coupon behaviour    |
| 06  | Transaction Discount Analysis | Analyzing discounts and transactions       |
| 07  | Dataset Integration           | Combining relevant datasets                |

### Phase 2: Treatment and Outcome Analysis

| Day | Notebook                      | Objective                                 |
| --- | ----------------------------- | ----------------------------------------- |
| 08  | Treatment Outcome Analysis    | Exploring treatment and outcome variables |
| 09  | Campaign Exposure Analysis    | Investigating campaign exposure           |
| 10  | Customer Campaign Analysis    | Studying customer-campaign relationships  |
| 11  | Treatment Outcome Definition  | Defining treatment and outcomes           |
| 12  | Treatment Assignment Analysis | Investigating treatment assignment        |
| 13  | Customer Exposure Analysis    | Examining customer-level exposure         |

### Phase 3: Causal Identification and Validation

| Day | Notebook                       | Objective                                   |
| --- | ------------------------------ | ------------------------------------------- |
| 14  | Causal Identification          | Assessing causal identification feasibility |
| 15  | Treatment Assignment Evidence  | Evaluating treatment assignment evidence    |
| 16  | Dataset Documentation          | Documenting data and causal design          |
| 17  | Treatment Definition           | Refining treatment definitions              |
| 18  | Dataset Documentation Research | Consolidating dataset research              |
| 19  | Transaction Outcome Validation | Validating transaction outcomes             |
| 20  | Transaction Measurement        | Assessing outcome measurement feasibility   |

---

## 🤖 Machine Learning Model

EconoCausal uses a **Random Forest Classifier** to predict customer coupon redemption.

### Model Architecture

The trained model uses a Scikit-learn Pipeline.

**1. Numerical Preprocessing**

* SimpleImputer (Median Strategy)
* StandardScaler

**2. Categorical Preprocessing**

* SimpleImputer (Most Frequent Strategy)
* OneHotEncoder

**3. Classification Algorithm**

* RandomForestClassifier

### Model Configuration

```python
RandomForestClassifier(
    class_weight='balanced',
    max_depth=15,
    min_samples_leaf=10,
    min_samples_split=10,
    n_jobs=-1,
    random_state=42
)
```

### Important Model Features

* Campaign Type
* Customer Demographics
* Purchase Frequency
* Total Quantity
* Total Spending
* Average Spending
* Coupon Discount
* Other Discount
* Campaign Duration
* Campaign Start Month
* Campaign Start Year
* Product Diversity

### Target Distribution

The training dataset contains:

| Redemption Status | Records |
| ----------------- | ------: |
| 0 (Not Redeemed)  |  77,640 |
| 1 (Redeemed)      |     729 |
| Total             |  78,369 |

The dataset has significant class imbalance. Therefore, balanced class weights were incorporated into the Random Forest classifier.

---

## 📈 Causal Analysis

One of the most important components of EconoCausal is its investigation of causal relationships.

The project explores the following question:

**How much does customer purchasing behaviour change when a promotional offer is given?**

The intended causal framework is:

* Treatment: Receiving a promotional offer.
* Control: Not receiving the promotional offer.
* Outcome: Customer purchasing behaviour.
* Treatment Effect: Difference in outcomes attributable to receiving the offer.

However, identifying actual offer exposure and treatment assignment is essential.

The available dataset did not establish sufficiently reliable treatment-assignment evidence.

Therefore:

* Campaign types X and Y were not automatically treated as experimental treatment and control groups.
* Coupon redemption was not considered proof of offer assignment.
* Transaction discounts alone were not considered sufficient evidence of offer exposure.
* Numerical causal treatment effects were not reported.

This distinction prevents misleading business conclusions.

### Future Causal Analysis

With verified treatment-assignment data, the project can be extended using:

* Average Treatment Effect (ATE)
* Conditional Average Treatment Effect (CATE)
* Double Machine Learning (DML)
* Uplift Modelling
* Treatment Effect Heterogeneity

---

## 🚀 Streamlit Deployment

EconoCausal includes a Streamlit application for presenting the machine learning project.

### Application Features

* EconoCausal project interface
* Customer coupon redemption prediction overview
* Machine learning model loading
* Model deployment status
* Project overview section

### Run Locally

Clone the repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Navigate to the project directory:

```bash
cd EconoCausal
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Launch the application:

```bash
streamlit run app.py
```

The application will be available at:

```text
http://localhost:8501
```

**Note:** The current verified Streamlit implementation loads the saved model and displays the project overview. A complete interactive prediction form requires additional implementation and testing.

---

## 📁 Project Structure

```text
EconoCausal/
│
├── data/
│   └── raw/
│
├── notebooks/
│   ├── 01_data_inspection.ipynb
│   ├── 02_data_quality_analysis.ipynb
│   ├── 03_dataset_relationships.ipynb
│   ├── 04_target_analysis.ipynb
│   ├── 05_customer_coupon_analysis.ipynb
│   ├── 06_transaction_discount_analysis.ipynb
│   ├── 07_dataset_integration.ipynb
│   ├── 08_treatment_outcome_analysis.ipynb
│   ├── 09_campaign_exposure_analysis.ipynb
│   ├── 10_customer_campaign_analysis.ipynb
│   ├── 11_treatment_outcome_definition.ipynb
│   ├── 12_treatment_assignment_analysis.ipynb
│   ├── 13_customer_exposure_analysis.ipynb
│   ├── 14_causal_identification.ipynb
│   ├── 15_treatment_assignment_evidence.ipynb
│   ├── 16_dataset_documentation.ipynb
│   ├── 17_treatment_definition.ipynb
│   ├── 18_dataset_documentation_research.ipynb
│   ├── 19_transaction_outcome_validation.ipynb
│   └── 20_transaction_measurement_outcome_feasibility.ipynb
│
├── models/
│   ├── econocausal_model.pkl
│   └── model_features.pkl
│
├── reports/
│
├── src/
│
├── tests/
│
├── app.py
├── requirements.txt
└── README.md
```

*The structure represents the project's main components; retain the actual notebook filenames and directory names from your repository.*

---

## 📊 Key Project Outcomes

The project successfully established:

1. A structured 20-notebook data science workflow.
2. Comprehensive exploration of customer, campaign, coupon, and transaction datasets.
3. Identification of severe class imbalance in redemption behaviour.
4. A Random Forest machine learning pipeline.
5. Model serialization using Joblib.
6. A documented causal identification feasibility assessment.
7. A Streamlit deployment prototype.
8. A foundation for future customer uplift and campaign effectiveness analysis.

Numerical predictive performance metrics and causal impact estimates remain to be validated before being reported.

---

## 🔮 Future Improvements

Potential improvements include:

* Complete interactive customer prediction functionality.
* Add customer-level redemption probability.
* Develop campaign effectiveness dashboards.
* Identify reliable treatment and control groups.
* Integrate verified offer-exposure information.
* Implement Double Machine Learning.
* Develop customer uplift segmentation.
* Estimate incremental revenue and customer spending when causal assumptions are satisfied.
* Deploy the application to Streamlit Community Cloud.

---

## 🎯 Project Vision

The long-term vision of EconoCausal is to move beyond traditional coupon redemption prediction toward understanding the actual incremental impact of marketing campaigns.

Rather than simply identifying customers who are likely to redeem coupons, the system aims to help businesses understand which customers genuinely change their purchasing behaviour because of promotional offers.

**Predict customer behaviour. Understand campaign impact. Enable smarter marketing decisions.**

---

## 👨‍💻 Author

**Keshav Dev Gaur**

B.Tech – Computer Science and Engineering (AI/ML)

Interested in:

* Machine Learning
* Data Science
* Artificial Intelligence
* Causal Inference
* Predictive Analytics

---

⭐ If you find this project interesting, consider giving the repository a star!

**EconoCausal – From Coupon Prediction to Causal Marketing Intelligence.**
