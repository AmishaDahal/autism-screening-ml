# Autism Spectrum Disorder Screening Using Machine Learning

## Overview
This project explores the use of machine learning techniques to support early screening of Autism Spectrum Disorder (ASD) in children. The goal is not to replace clinical diagnosis, but to build a practical and interpretable screening-support system that can help identify potential ASD cases earlier.

## Objective
The main objective of this project is to analyze behavioral and demographic screening data and develop classification models that can distinguish between ASD-positive and ASD-negative cases. Because ASD screening is a healthcare-related task, special emphasis was placed on recall so that fewer positive cases are missed.

## Dataset
This project uses the **Autistic Spectrum Disorder Screening Data for Children** dataset from the UCI Machine Learning Repository.

Dataset source:  
[UCI Machine Learning Repository – ASD Screening Data for Children](https://archive.ics.uci.edu/)

The dataset includes:
- Behavioral screening questions (A1–A10)
- Demographic features
- Family and medical background variables
- Binary ASD outcome label

## Methods
The project includes:
- Data cleaning and preprocessing
- Exploratory Data Analysis (EDA)
- Handling class imbalance
- Feature selection and interpretation
- Model training and evaluation using:
  - Logistic Regression
  - Random Forest
  - AdaBoost
  - XGBoost

## Evaluation
Because this is a screening problem, model evaluation focused on:
- Recall
- Precision
- F1-score
- F2-score
- ROC-AUC
- PR-AUC
- Confusion Matrix

Threshold optimization was performed to compare performance under both F1 and F2 criteria.

## Key Findings
- Behavioral features, especially **A2–A9**, were the strongest predictors.
- Threshold optimization improved screening performance by increasing recall.
- Ensemble models performed strongly overall.
- **Random Forest under F2 optimization** gave the best screening-oriented performance.
- **Logistic Regression** remained one of the most interpretable and stable models.

## Best Model
The best model for screening performance was:

**Random Forest (F2-optimized threshold)**

This model achieved the strongest recall-oriented performance, making it most suitable for screening support.

## Project Files
- `report/final_report.pdf` – Final report
- `notebooks/` – Analysis notebooks
- `src/` – Python scripts
- `figures/` – Visualizations used in the report

## Important Note
This project is intended for **educational and research purposes only**. It is not a diagnostic tool and should not be used as a substitute for professional clinical evaluation.

## Author
Amisha Dahal
