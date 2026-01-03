# Loan Default Prediction

## Overview
Machine learning classification project to predict loan defaults for a microfinance institution using Lending Club data.

## Business Problem
**Stakeholder:** Risk Management Team at a Microfinance Institution

**Goal:** Predict which loan applicants are likely to default to minimize financial losses.

## Dataset
- Source: Lending Club (2007-2018 Q4)
- Size: 10,000 loans
- Features: 6 numeric features (loan amount, interest rate, income, DTI, accounts)
- Target: Binary (Default = 1, No Default = 0)
- Default rate: 17.8%

## Methodology
1. Exploratory Data Analysis with 5 visualizations
2. Data preprocessing (handling missing values, scaling)
3. Train-test split (80/20)
4. Built 3 models:
   - Baseline: Logistic Regression
   - Decision Tree (max_depth=5)
   - Tuned Decision Tree (hyperparameter optimization)

## Results
**Best Model:** Tuned Decision Tree
- Accuracy: 81.0%
- Precision: 27.7%
- Recall: 11.2%
- F1-Score: 0.159

## Key Findings
- Interest rate and DTI are the most important predictors
- Class imbalance limits model performance
- Model catches 11% of defaults (low recall)

## Recommendations
1. Use model as a screening tool, not final decision maker
2. Combine predictions with manual review
3. Address class imbalance with advanced techniques
4. Collect more data on defaulted loans

## Repository Structure
```
├── data/                      # Dataset files (not tracked)
├── images/                    # Visualizations (8 charts)
├── notebook.ipynb             # Full analysis notebook
├── presentation.pdf           # Non-technical presentation
└── README.md                  # Project documentation
```

## Technologies Used
- Python 3.x
- pandas, numpy
- scikit-learn
- matplotlib, seaborn

## Author
Jose Barasa - Moringa School Data Science Phase 3 Project

## Date
December 23, 2025