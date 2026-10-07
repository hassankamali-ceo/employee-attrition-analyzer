# Employee Attrition Analyzer

**Lab 7 — Open Ended Lab (Machine Learning)**

| | |
|---|---|
| **Project Name** | Employee Attrition Analyzer |
| **Name** | M. Hassan |
| **Roll No** | 24F-AI-065 |
| **Dataset** | IBM HR Analytics Employee Attrition & Performance |

## Description

This project analyzes the IBM HR Analytics Employee Attrition & Performance dataset
(1470 employee records, 35 features) to predict whether an employee will leave the
company (Attrition = Yes/No).

## Files

| File | Description |
|---|---|
| `Employee_Attrition_Analyzer.ipynb` | Main Jupyter notebook — complete, fully commented code with outputs |

## What the notebook contains

1. **Dataset description** — IBM HR Analytics dataset overview
2. **EDA & visualization** — attrition distribution, attrition by department/overtime, age distribution
3. **Preprocessing** — dropping useless columns (`EmployeeCount`, `Over18`, `StandardHours`, `EmployeeNumber`),
   label encoding the target, one-hot encoding categorical features, 80/20 stratified train-test split,
   feature scaling with `StandardScaler`
4. **ML models** — Logistic Regression, Decision Tree, Random Forest (all trained on the same preprocessed data)
5. **Evaluation** — accuracy, precision, recall, F1 score comparison table, confusion matrices for all three models,
   classification report
6. **Feature importance** — top-15 feature importance bar chart from the Random Forest

## Results

- **Logistic Regression** performed best: ~86% accuracy and the highest F1 score for the "Leave" class.
- Strongest attrition drivers: **OverTime, MonthlyIncome, Age, TotalWorkingYears, YearsAtCompany**.

## How to run

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

1. Download the dataset `WA_Fn-UseC_-HR-Employee-Attrition.csv` (search
   "IBM HR Analytics Employee Attrition & Performance" on Kaggle) and place it
   in the same folder as the notebook.
2. Open the notebook in Jupyter and run all cells top to bottom.

> Note: the notebook in this repo keeps the code and text outputs; plot images
> were removed to keep the repository light. Run the notebook locally to
> reproduce all charts.
