# insurance-claim-prediction
│
├── data/
│   ├── Train_data.xlsx
│   └── Variable_Description.xlsx
│
├── notebooks/
│   ├── 01_exploratory_data_analysis.ipynb
│   └── 02_modeling_and_evaluation.ipynb
│
├── results/
│   └── model_performance.csv
│
├── requirements.txt
└── README.md
# Insurance Claim Prediction Project

## Overview
This project aims to predict the probability that a building will experience
at least one insurance claim during its insured period based on building characteristics.

## Business Problem
Insurance companies need to accurately assess building risk to:
- Price premiums correctly
- Manage portfolio risk
- Reduce unexpected claim exposure

## Target Variable
- Claim = 1 → Building had at least one claim
- Claim = 0 → No claim during insured period

## Methodology
1. Data Cleaning & Preprocessing
2. Exploratory Data Analysis (EDA)
3. Feature Engineering
4. Model Training:
   - Logistic Regression
   - Random Forest
   - Gradient Boosting
5. Model Evaluation using ROC-AUC

## Results
Gradient Boosting achieved the best overall performance:
- Accuracy ≈ 78.5%
- ROC-AUC ≈ 0.69

ROC-AUC was prioritized due to class imbalance in insurance claims.

## Tools & Libraries
- Python
- pandas, numpy
- scikit-learn
- matplotlib, seaborn
