# Liver-Patient-Dataset
Predicting liver disease using Logistic Regression, Random Forest &amp; XGBoost — with SMOTE, SHAP explainability, and full model comparison (ILPD dataset)
## Overview
Liver disease cases have been steadily rising due to alcohol consumption, 
exposure to harmful substances, contaminated food, and drug use. This project 
builds and compares machine learning models to predict liver disease from 
clinical and biochemical markers, aiming to support early diagnosis and 
reduce the burden on doctors.

## Dataset
Indian Liver Patient Dataset (ILPD) — 10 clinical features including Age, 
Gender, Bilirubin levels, liver enzymes (SGOT/SGPT), Total Proteins, and 
Albumin ratios, with a binary target: disease present or not.

## Approach
- **EDA**: Explored demographics, enzyme levels, and protein markers to 
  understand feature distributions and relationships with disease outcome
- **Feature Engineering**: Created bilirubin ratio, enzyme ratio, protein 
  balance, log-transformed skewed features, and age-albumin interaction terms
- **Class Imbalance**: Applied SMOTE to handle the disease/no-disease imbalance
- **Models**: Logistic Regression, Random Forest, and XGBoost
- **Evaluation**: Accuracy, Precision, Recall, F1-score, ROC-AUC, 
  Precision-Recall curves, and Calibration curves
- **Explainability**: SHAP values to interpret XGBoost's predictions — 
  critical for trust in medical ML applications

## Results
| Model | Strength |
|---|---|
| Logistic Regression | Most interpretable, useful for medical decision-making |
| Random Forest | Balanced, robust baseline |
| XGBoost | Best F1-score and predictive power after tuning |

**Conclusion**: XGBoost with SMOTE performed best overall, but Logistic 
Regression remains valuable where interpretability matters more than raw 
accuracy — a common trade-off in healthcare ML.

## Tech Stack
Python · Pandas · NumPy · Scikit-learn · XGBoost · SHAP · Seaborn · Matplotlib
