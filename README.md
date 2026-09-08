# Lab 3: Decision Tree Classification — Telco Customer Churn

## Overview
This project builds and evaluates a Decision Tree classifier to predict customer churn 
using the Telco Customer Churn dataset. It covers the full workflow: feature preparation, 
train/test splitting, baseline model training, evaluation, an overfitting investigation 
across tree depths, model selection, and feature importance interpretation.

## Contents
- `lab3_Manahil_Fatima_churn_dt.ipynb` — main notebook with all tasks and analysis
- `clean_churn.csv` — cleaned dataset from Lab 2 (EDA & data cleaning)

## Workflow
1. **Feature & Target Preparation** — encoded categorical variables, separated target (`Churn`)
2. **Train/Test Split** — 80/20 stratified split to preserve class balance
3. **Baseline Decision Tree** — trained an unrestricted tree as a starting point
4. **Model Evaluation** — accuracy, precision, recall, F1-score, confusion matrix
5. **Overfitting Investigation** — compared train vs. test accuracy across multiple `max_depth` values
6. **Model Selection** — chose the depth that best balances train/test performance
7. **Feature Importance** — identified top predictors of churn and connected them back to EDA findings

## Key Findings
- Customer **tenure**, **internet service type**, and **payment method** are the strongest predictors of churn.
- The unrestricted baseline tree overfit significantly; limiting `max_depth` improved generalization.
- Since churn is imbalanced (~73% No / ~27% Yes), recall and F1-score were prioritized over raw accuracy.

## Tools Used
Python, Pandas, NumPy, scikit-learn, Matplotlib, Seaborn, Google Colab

## Author
[Manahil Fatima] — BS Computer Science, 5th Semester  
