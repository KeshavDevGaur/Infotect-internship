# 📓 EconoCausal – Notebooks Documentation

This directory contains the complete Jupyter Notebook workflow for **EconoCausal: Customer Coupon Redemption Prediction & Causal Campaign Analysis**.

The notebooks document the project's development from raw dataset exploration to causal feasibility assessment, machine learning preparation, and model development.

---

## 🎯 Notebook Objectives

The notebooks were developed to:

* Understand customer coupon redemption behaviour.
* Explore customer demographics and purchasing patterns.
* Analyze promotional campaigns and coupon-item relationships.
* Integrate multiple datasets.
* Investigate treatment assignment and campaign exposure.
* Evaluate causal identification feasibility.
* Prepare features for machine learning.
* Develop and interpret a coupon redemption prediction model.

---

## 📂 Notebook Structure

### Phase 1: Data Understanding and Exploration

| No. | Notebook                      | Description                                                              |
| --- | ----------------------------- | ------------------------------------------------------------------------ |
| 01  | Data Inspection               | Initial dataset exploration, dimensions, columns, and data types.        |
| 02  | Data Quality Analysis         | Missing values, duplicate records, and data consistency.                 |
| 03  | Dataset Relationships         | Understanding relationships between source datasets.                     |
| 04  | Target Analysis               | Analysis of coupon redemption status and class distribution.             |
| 05  | Customer Coupon Analysis      | Exploring customer and coupon relationships.                             |
| 06  | Transaction Discount Analysis | Investigating customer transactions and discount behaviour.              |
| 07  | Dataset Integration           | Combining customer, campaign, coupon, item, and transaction information. |

### Phase 2: Treatment and Outcome Analysis

| No. | Notebook                      | Description                                            |
| --- | ----------------------------- | ------------------------------------------------------ |
| 08  | Treatment Outcome Analysis    | Exploring candidate treatment and outcome variables.   |
| 09  | Campaign Exposure Analysis    | Investigating available campaign exposure information. |
| 10  | Customer Campaign Analysis    | Studying customer-campaign relationships.              |
| 11  | Treatment Outcome Definition  | Defining candidate treatment and outcome variables.    |
| 12  | Treatment Assignment Analysis | Investigating treatment assignment evidence.           |
| 13  | Customer Exposure Analysis    | Examining customer-level exposure information.         |

### Phase 3: Causal Identification and Validation

| No. | Notebook                                    | Description                                                             |
| --- | ------------------------------------------- | ----------------------------------------------------------------------- |
| 14  | Causal Identification                       | Assessing whether causal effects can be identified.                     |
| 15  | Treatment Assignment Evidence               | Evaluating available evidence about treatment assignment.               |
| 16  | Dataset Documentation                       | Documenting dataset structure and causal design considerations.         |
| 17  | Treatment Definition                        | Refining treatment definitions and identification strategy.             |
| 18  | Dataset Documentation Research              | Consolidating dataset research and documentation.                       |
| 19  | Transaction Outcome Validation              | Validating transaction-based outcome measurements.                      |
| 20  | Transaction Measurement Outcome Feasibility | Assessing whether transaction data supports causal outcome measurement. |

---

## 🤖 Machine Learning Development

The later project workflow extends beyond the initial 20 analysis notebooks.

The machine learning development phase includes:

| Day | Notebook               | Objective                                                               |
| --- | ---------------------- | ----------------------------------------------------------------------- |
| 26  | ML Dataset Preparation | Date conversion, historical customer features, and dataset preparation. |
| 27  | Feature Engineering    | Feature selection, missing-value checks, and feature preparation.       |
| 28  | ML Model Training      | Training Logistic Regression and Random Forest models.                  |
| 29  | Model Evaluation       | Comparing classification performance and confusion matrices.            |
| 30  | Hyperparameter Tuning  | Optimizing Random Forest parameters using cross-validation.             |
| 31  | Model Explainability   | Using SHAP to interpret model predictions.                              |
| 32  | Model Deployment       | Saving the trained model and preparing Streamlit deployment.            |

**Note:** Day 32 covers the initial deployment implementation. The complete interactive prediction workflow remains future work.

---

## 🧠 Machine Learning Techniques

The project uses:

* Logistic Regression
* Random Forest Classifier
* Class Weight Balancing
* Feature Engineering
* One-Hot Encoding
* Standard Scaling
* Hyperparameter Optimization
* SHAP Explainability

### Final Saved Model

```text
models/
├── econocausal_model.pkl
└── model_features.pkl
```

The saved Random Forest pipeline includes preprocessing and classification components.

---

## 🔬 Causal Analysis Techniques

The notebooks investigate:

* Treatment and control definitions
* Campaign exposure
* Treatment assignment
* Customer exposure
* Outcome measurement
* Causal identification feasibility

Potential future techniques:

* Average Treatment Effect (ATE)
* Conditional Average Treatment Effect (CATE)
* Double Machine Learning (DML)
* Uplift Modelling
* Counterfactual Analysis

**Important:** The current dataset analysis did not establish sufficiently reliable treatment-assignment evidence. Therefore, numerical causal treatment effects have not been reported.

---

## 🛠️ Tools and Libraries

| Tool         | Purpose                   |
| ------------ | ------------------------- |
| Python       | Programming               |
| JupyterLab   | Notebook development      |
| Pandas       | Data manipulation         |
| NumPy        | Numerical operations      |
| Matplotlib   | Data visualization        |
| Seaborn      | Statistical visualization |
| Scikit-learn | Machine learning          |
| SHAP         | Model explainability      |
| Joblib       | Model serialization       |
| Streamlit    | Application deployment    |

---

## 📊 Key Project Findings

1. The dataset contains 78,369 labelled training records.
2. Only 729 records belong to the positive redemption class.
3. The positive class represents approximately 0.93% of the training data.
4. Class imbalance is an important consideration for model training and evaluation.
5. A Random Forest classification pipeline was developed and saved.
6. SHAP analysis was used to investigate feature contributions.
7. Treatment assignment and offer exposure require stronger evidence before causal impact can be estimated.

---

## 📁 Related Project Directories

```text
EconoCausal/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│   ├── README.md
│   ├── 01_data_inspection.ipynb
│   ├── ...
│   └── 32_model_deployment.ipynb
│
├── models/
│   ├── econocausal_model.pkl
│   └── model_features.pkl
│
├── reports/
│   ├── README.md
│   └── final_project_report.pdf
│
├── app.py
├── requirements.txt
└── README.md
```

*Use the actual filenames in your repository when organizing the notebooks.*

---

## 🏁 Conclusion

The notebook collection represents the complete analytical development of EconoCausal, covering data exploration, customer behaviour analysis, causal feasibility research, feature engineering, machine learning, model evaluation, explainability, and initial deployment.

The project establishes a foundation for developing an intelligent marketing analytics platform capable of predicting coupon redemption and, with suitable treatment-assignment data, estimating the actual incremental impact of promotional campaigns.

---

**Project:** EconoCausal
**Author:** Keshav Dev Gaur
**Domain:** Data Science | Machine Learning | Causal Analysis

**EconoCausal – From Coupon Prediction to Causal Marketing Intelligence.**
