# Healthcare Readmission Prediction & Analytics

An end-to-end healthcare data analytics and machine learning project focused on analyzing patient data and predicting **30-day hospital readmission risk**.

The project processes more than **100,000 patient records**, performs data preprocessing and exploratory data analysis, builds and compares machine learning classification models, generates visual insights, and develops a risk-stratification framework for healthcare decision support.

---

## 📌 Project Overview

Hospital readmissions within 30 days can increase healthcare costs and place additional pressure on healthcare resources.

This project aims to analyze patient and healthcare-related data to identify patterns associated with readmission and build a predictive model that can help identify patients who may be at higher risk of readmission.

The project follows an end-to-end workflow:

**Data Processing → EDA → Visualization → Machine Learning → Model Evaluation → Risk Stratification → Business Insights**

---

## 🎯 Objectives

- Analyze a large healthcare dataset containing patient records and clinical features.
- Clean and preprocess the data for analysis and modeling.
- Explore patterns and relationships associated with 30-day readmission.
- Visualize important characteristics of the dataset.
- Train multiple machine learning classification models.
- Compare model performance using appropriate evaluation metrics.
- Identify important features influencing predictions.
- Develop a patient risk-stratification framework.
- Generate actionable business and healthcare insights.
- Document the complete project for reproducibility.

---

## 📊 Dataset

The project uses a healthcare dataset containing:

| Attribute | Value |
|---|---:|
| Patient records | 101,766 |
| Features | 50 |
| Target | 30-day readmission |
| Readmitted patients | 11,357 |
| Non-readmitted patients | 90,409 |
| Readmission rate | 11.16% |

The dataset was cleaned and prepared before analysis.

### Data Preprocessing

The preprocessing workflow included:

- Handling missing values
- Addressing placeholder values
- Encoding categorical variables
- Validating data quality
- Preparing the dataset for machine learning

A total of **9 categorical features were encoded**.

The final cleaned dataset contains **101,766 rows and 50 columns**. :contentReference[oaicite:1]{index=1}

> **Note:** The raw dataset is not included in the repository if its size or distribution restrictions make direct GitHub hosting impractical. Download instructions can be provided separately in the project documentation.

---

## 🔎 Exploratory Data Analysis

A comprehensive Exploratory Data Analysis (EDA) was performed to understand the structure of the dataset and identify relationships with the target variable.

The analysis includes:

- Target variable distribution
- Numeric feature distributions
- Categorical feature distributions
- Numeric variables vs. readmission
- Categorical variables vs. readmission
- Correlation analysis
- Feature relationships
- Readmission patterns
- Risk-related patterns

The project generated **12 visualizations** covering both exploratory analysis and machine learning results. :contentReference[oaicite:2]{index=2}

---

## 🤖 Machine Learning

Two classification algorithms were trained and evaluated:

### 1. Logistic Regression

A baseline classification model used to predict the probability of 30-day readmission.

### 2. Random Forest Classifier

An ensemble machine learning model used to capture more complex relationships between patient characteristics and readmission risk.

### Best Performing Model

The **Random Forest Classifier** performed better among the evaluated models.

| Metric | Random Forest |
|---|---:|
| ROC AUC | 0.6529 |
| Accuracy | 0.7553 |
| Precision | 0.1948 |
| Recall | 0.3809 |

Because the target variable is imbalanced, multiple evaluation metrics were considered instead of relying only on accuracy. :contentReference[oaicite:3]{index=3}

---

## 📈 Model Analysis

The project includes several model-analysis outputs:

- Model performance comparison
- Confusion matrices
- Feature importance analysis
- Prediction probability distribution
- Risk stratification
- Model evaluation metrics

These outputs help interpret model performance and understand how predictions can be used for risk identification. :contentReference[oaicite:4]{index=4}

---

## ⚠️ Risk Stratification

A risk-stratification framework was developed using model predictions and probability scores.

The framework categorizes patients based on predicted readmission risk and can be used to support prioritization of patients who may require additional attention.

The analysis identified **865 high-risk patients** within the analyzed dataset. :contentReference[oaicite:5]{index=5}

> The model is intended as a decision-support tool and should not replace professional clinical judgment.

---

## 💼 Business Insights

The project demonstrates how healthcare analytics and machine learning can support data-driven decision-making.

Potential applications include:

- Identifying high-risk patients
- Supporting targeted follow-up
- Prioritizing healthcare resources
- Understanding readmission patterns
- Supporting intervention planning
- Improving risk-monitoring processes

The project also includes a cost-benefit analysis framework with an estimated potential cost-saving opportunity of **$4,642,500**, based on the project's assumptions. :contentReference[oaicite:6]{index=6} :contentReference[oaicite:7]{index=7}

---

## 📊 Visualizations

The project contains 12 generated visualizations:

```text
visualizations/
│
├── 01_target_distribution.png
├── 02_numeric_distributions.png
├── 03_categorical_distributions.png
├── 04_numeric_vs_readmission.png
├── 05_categorical_vs_readmission.png
├── 06_correlation_matrix.png
├── 07_model_comparison.png
├── 08_confusion_matrices.png
├── 09_feature_importance.png
├── 10_probability_distribution.png
├── 11_risk_stratification.png
└── 12_FINAL_DASHBOARD.png
