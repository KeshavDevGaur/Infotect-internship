# 📑 EconoCausal – Project Reports

This directory contains the final documentation, analysis summaries, research findings, and project reports for **EconoCausal: Customer Coupon Redemption Prediction & Causal Campaign Analysis**.

The reports document the complete development journey, from initial dataset exploration to machine learning model development and deployment.

---

## 📂 Reports Directory Structure

```text
reports/
│
├── README.md
│
├── project_overview.md
│
├── data_analysis_report.md
│
├── feature_engineering_report.md
│
├── causal_analysis_report.md
│
├── model_development_report.md
│
├── model_evaluation_report.md
│
├── deployment_report.md
│
└── final_project_report.pdf
```

*These filenames represent the recommended documentation structure. Keep only files that actually exist in the repository.*

---

## 1. Project Overview

**EconoCausal** is a data science project focused on understanding customer coupon redemption behaviour and investigating the impact of promotional campaigns.

The project combines:

* Exploratory Data Analysis
* Customer Behaviour Analysis
* Data Integration
* Feature Engineering
* Machine Learning
* Causal Identification Research
* Model Explainability
* Streamlit Deployment

### Main Objective

To develop a predictive system that estimates customer coupon redemption and establish a foundation for measuring the incremental impact of promotional offers.

---

## 2. Data Analysis Reports

The initial analysis phase covers:

* Dataset inspection
* Data quality assessment
* Missing value analysis
* Duplicate detection
* Dataset relationships
* Customer demographics
* Coupon redemption distribution
* Campaign analysis
* Transaction and discount analysis

**Dataset:** AmExpert 2019 Marketing Campaign Dataset.

---

## 3. Causal Analysis Reports

The causal analysis phase investigates whether promotional offers actually change customer purchasing behaviour.

Important research areas:

* Treatment and outcome definition
* Campaign exposure analysis
* Customer exposure analysis
* Treatment assignment investigation
* Causal identification feasibility
* Transaction outcome validation
* Transaction measurement feasibility

### Important Finding

The available dataset did not establish sufficiently reliable treatment-assignment or offer-exposure evidence.

Therefore, causal treatment effects and incremental revenue estimates have not been claimed.

Future research can explore:

* Average Treatment Effect (ATE)
* Conditional Average Treatment Effect (CATE)
* Double Machine Learning
* Uplift Modelling
* Counterfactual Analysis

---

## 4. Machine Learning Reports

The machine learning phase focuses on predicting customer coupon redemption.

### Model Development

**Algorithm:** Random Forest Classifier

**Preprocessing:**

* Simple Imputer
* Standard Scaler
* One-Hot Encoding

**Model Configuration:**

* Class Weight: Balanced
* Maximum Depth: 15
* Random State: 42

### Model Artifacts

```text
models/
│
├── econocausal_model.pkl
└── model_features.pkl
```

The trained pipeline is serialized using Joblib.

The dataset has significant class imbalance, with approximately 0.93% positive redemption records.

Numerical model evaluation metrics must be taken from reproducible validation results rather than assumed.

---

## 5. Model Explainability

SHAP was used to investigate feature contributions to model predictions.

The analysis focuses on:

* Feature importance
* Customer purchasing behaviour
* Campaign characteristics
* Model prediction interpretation

SHAP explanations describe model behaviour; they do not independently establish causal relationships.

---

## 6. Deployment Report

EconoCausal includes a Streamlit application.

### Deployment Components

* Project dashboard
* Machine learning model loading
* Model status verification
* Project overview

### Run Application

```bash
streamlit run app.py
```

Local application:

```text
http://localhost:8501
```

The verified deployment currently loads the saved model and displays the project overview. Full interactive prediction functionality requires further integration and testing.

---

## 7. Final Project Deliverables

| Deliverable                            | Status      |
| -------------------------------------- | ----------- |
| Dataset Exploration                    | Completed   |
| Data Quality Analysis                  | Completed   |
| Dataset Integration                    | Completed   |
| Customer Behaviour Analysis            | Completed   |
| Causal Feasibility Investigation       | Completed   |
| Feature Engineering                    | Completed   |
| Random Forest Model Training           | Completed   |
| Hyperparameter Tuning                  | Completed   |
| SHAP Explainability                    | Completed   |
| Model Serialization                    | Completed   |
| Streamlit Initial Deployment           | Completed   |
| Verified Causal Impact Estimation      | Future Work |
| Complete Interactive Prediction System | Future Work |

---

## 8. Future Improvements

Planned improvements include:

1. Complete interactive ML prediction functionality.
2. Improve model evaluation and validation.
3. Integrate reliable campaign exposure information.
4. Develop customer uplift modelling.
5. Implement Double Machine Learning where assumptions are satisfied.
6. Estimate incremental customer spending.
7. Develop campaign effectiveness dashboards.
8. Deploy the application publicly.

---

## 9. Final Conclusion

EconoCausal establishes a foundation for intelligent marketing analytics by combining customer behaviour analysis, coupon redemption prediction, causal feasibility research, and machine learning deployment.

The project highlights an important distinction between predicting customer redemption and measuring the actual impact of promotional offers.

Its long-term objective is to help businesses identify not only customers likely to redeem coupons, but also customers whose purchasing behaviour genuinely changes because of promotional incentives.

---

**Project:** EconoCausal
**Author:** Keshav Dev Gaur
**Domain:** Machine Learning | Data Science | Causal Analysis
**Dataset:** AmExpert 2019 Marketing Campaign

**EconoCausal – From Coupon Prediction to Causal Marketing Intelligence.**
