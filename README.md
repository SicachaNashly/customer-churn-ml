# Customer Churn Prediction — Notebook (scikit-learn)

This repository contains a Jupyter Notebook that trains a baseline **churn** model and scores new rows using a clean scikit-learn pipeline.

**What it does:**
- Generates or loads an English CSV (`data/churn.csv`)
- Trains a pipeline: `OneHotEncoder + StandardScaler + LogisticRegression`
- Reports AUC, classification report, and shows a confusion matrix
- Saves the model (`models/model.pkl`)
- Scores a sample CSV and writes `reports/scored.csv`

## How to run
1) Open `Project2_Churn_Notebook.ipynb` in Jupyter/Colab.
2) Run cells top-to-bottom. If `data/churn.csv` is missing, the notebook creates a synthetic dataset automatically.
3) Outputs:
   - `models/model.pkl`
   - `reports/scored.csv`
   - confusion matrix plot in the notebook

## Structure (recommended)
customer-churn-ml/
├─ Project2_Churn_Notebook.ipynb
├─ data/ # created/used by the notebook
├─ models/ # model.pkl (after training)
├─ reports/ # scored.csv (after scoring)
└─ assets/ # optional screenshots for README

## Tech
Python, pandas, scikit-learn, joblib, matplotlib.
