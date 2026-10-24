# Telco-Customer-Churn-Prediction
End-to-end machine learning project for customer churn prediction using Python, scikit-learn, feature engineering, model comparison, and hyperparameter tuning.

## Overview

An end-to-end machine learning project that predicts telecommunications customer churn using demographic, subscription, and billing information.

The project covers exploratory data analysis, preprocessing, model comparison, hyperparameter tuning, and final evaluation.

## Dataset

**IBM Telco Customer Churn**

- Total records: 7,043
- Target: `Churn` (`Yes` / `No`)
- Approximately 26.5% of customers churned

## Technologies

Python, Pandas, NumPy, Matplotlib, Seaborn, scikit-learn, Jupyter Notebook.

## Machine Learning Models

- DummyClassifier
- Logistic Regression
- Decision Tree
- Random Forest
- HistGradientBoostingClassifier

## Methodology

1. Exploratory Data Analysis
2. Data Cleaning and Preprocessing
3. Stratified Train/Test Split
4. Five-Fold Cross-Validation
5. Model Comparison
6. Hyperparameter Optimization
7. Final Test Evaluation

## Final Results

**Selected model:** Logistic Regression (`C=10`)

| Metric | Test Performance |
|---|---:|
| Accuracy | 80.20% |
| Precision | 64.80% |
| Recall | 55.61% |
| F1-score | 59.86% |
| ROC-AUC | 85.16% |

The model correctly identified 208 churners out of 374 actual churners in the test dataset.

## Key Findings

Logistic Regression achieved the highest cross-validation F1-score among the evaluated configurations.

The results indicate useful predictive performance, although approximately 44.4% of churners remain undetected at the evaluated classification threshold.

## Limitations and Future Improvements

- Explore classification-threshold optimization.
- Evaluate cost-sensitive classification.
- Assess probability calibration.
- Investigate additional predictive features.
- Evaluate generalization on external or more recent customer datasets.

## How to Run

1. Clone the repository.
2. Create and activate a Python virtual environment.
3. Install packages listed in `requirements.txt`.
4. Open `notebooks/customer_churn_analysis.ipynb`.
5. Run the notebook cells in order.

The CSV file must be available in the expected data directory before execution.