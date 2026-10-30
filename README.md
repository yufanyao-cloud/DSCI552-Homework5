# Homework 5: Decision Trees and Regression

This repository contains the solution notebook for DSCI 552 Homework 5.

## Contents

- data/: supplied data and descriptions
- notebook/Homework5_Decision_Trees_and_Regression.ipynb: complete solution
- requirements.txt: Python packages
- .github/workflows/run-notebook.yml: notebook check on GitHub Actions

## Data sources

- Acute Inflammations data set: UCI Machine Learning Repository.
- Communities and Crime data set: UCI Machine Learning Repository.

The input files are included in data/. The notebook reads them with relative paths only.

## Run the notebook

Use Python 3.10 or newer.

    python -m venv .venv
    .venv\Scripts\Activate.ps1
    pip install -r requirements.txt
    jupyter notebook notebook/Homework5_Decision_Trees_and_Regression.ipynb

To execute it from the repository root:

    jupyter nbconvert --to notebook --execute --inplace notebook/Homework5_Decision_Trees_and_Regression.ipynb

The notebook uses the first 1495 rows of Communities and Crime as training data and the remaining rows as test data. Randomized cross-validation uses random_state=552.