# Kaggle_ML_Hackathon

## Project Overview

This repository contains my solution for the M4 Practical Machine Learning Hackathon.  
The objective of the competition is to develop a robust binary classifier to predict loan default and maximize the F1-score on the test dataset.

The project emphasizes:

- Reliable model validation
- Class imbalance handling
- Threshold optimization for F1-score
- Business interpretation of prediction trade-offs

---

## Methodology

### 1. Data Processing
- Missing value imputation (median / most frequent)
- One-hot encoding for categorical features
- Feature-type separation via ColumnTransformer
- Stratified K-Fold cross-validation

### 2. Modeling Strategy
- Baseline models: Logistic Regression, Random Forest
- Final model: Regularized LightGBM
- Class imbalance handled via `scale_pos_weight`
- Fine-grained threshold tuning (not fixed at 0.5)

### 3. Model Evaluation
- Out-of-Fold (OOF) validation
- F1-score optimization
- Precision-Recall curve analysis
- Confusion matrix interpretation

---

## Final Model Highlights

- Stable LightGBM configuration
- Regularization to prevent overfitting
- Optimized decision threshold for F1-score
- Submission format:
  - Column 1: `ID` (starting from 1)
  - Column 2: `Predicted`

---

## Results

Public Leaderboard F1-score: **0.85+**

---

## Files

- `M4_Practice_Hackathon_Classifier.ipynb` — Main modeling notebook
- `README.md` — Project description

---

## Author

Runfei Wang  
