# DSCI 552 – Homework 5: Decision Trees, LASSO, and Boosting

## Contents

- **Acute Inflammations:** a label-powerset decision tree on a multi-label medical dataset, converted to IF-THEN rules and checked with cost-complexity pruning
- **Communities and Crime:** median imputation, correlation and coefficient-of-variation analysis, and regression with least squares, ridge, LASSO (raw and standardized), PCR, and L1-penalized XGBoost

## Results summary

| Model | Test MSE |
|---|---|
| XGBoost (L1, α = 0.1) | 0.0161 |
| Ridge | 0.0175 |
| LASSO | 0.0177 |
| LASSO (standardized) | 0.0177 |
| Least squares | 0.0180 |

The decision tree classifies all 120 patients correctly with 6 rules; pruning any further costs about 13 points of cross-validation accuracy.

## How to run

1. Download [Acute Inflammations](https://archive.ics.uci.edu/ml/datasets/Acute+Inflammations) and [Communities and Crime](https://archive.ics.uci.edu/ml/datasets/Communities+and+Crime) from UCI and unzip them inside the repo folder (the data is not included).
2. Install the dependencies: `pip install numpy pandas matplotlib seaborn scikit-learn xgboost`
3. Open `HW5.ipynb` and run all cells.
