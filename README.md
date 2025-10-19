# Alzheimer's Disease Prediction with Machine Learning

**Goal:** Develop an accurate, data-driven approach for predicting Alzheimer's disease presence and stage using patient health and cognitive data.

## Project Overview
This project applies tree-based machine learning models to identify Alzheimer's disease in patients using a synthetic clinical dataset from Kaggle. The goal is early diagnosis with strong predictive accuracy using diverse health and demographic inputs.

## Dataset
- 2,149 patient records, ages 60–90
- Features: demographics, lifestyle, medical history, clinical/cognitive measures, diagnosis (binary target)
- No missing values or duplicates; class ratio ~65:35 negative:positive

## Approach
- Data split: Stratified training/testing at 90/10, 80/20, 95/5
- Models: Decision Tree, Random Forest, XGBoost
- Hyperparameter tuning via GridSearchCV
- 5-fold cross-validation to evaluate robustness

## Key Findings
- Top predictors: MMSE, Functional Assessment, ADL scores
- Random Forest and XGBoost achieved highest accuracy (93%) and F1 scores (90%); Decision Tree excelled in recall
- Behavioral issues and memory complaints are linked to higher diagnosis risk 

## Recommendations
- Deploy the selected model as a clinical decision support tool.
- Periodically update the model with new patient data.
- Further refine model with expanded features and larger datasets.

## Limitations & Improvements
- Synthetic dataset means generalization to real patients should be validated
- Further feature engineering with expert insight may improve accuracy

## Resources
- [Report](https://github.com/thant-thiha/Alzheimers-Disease-Prediction/blob/main/Alzheimers-Disease-Prediction-Analytics.pdf)
- [Notebook](https://github.com/thant-thiha/Alzheimers-Disease-Prediction/blob/main/Alzheimers-Disease-Prediction.ipynb)
