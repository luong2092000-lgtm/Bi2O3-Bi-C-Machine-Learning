# Bi2O3-Bi-C-Machine-Learning
Machine learning prediction of short-term capacitance variations in Bi₂O₃/Bi@C electrodes
# Machine Learning Prediction of Capacitance Variations

This repository contains Python code and supporting data for predicting short-term changes in the specific capacitance of tea-waste-derived Bi₂O₃/Bi@C electrodes.

## Overview

The machine learning models estimate the percentage change in specific capacitance over the next 20 charge–discharge cycles (`Y_dCs20_pct`) using electrochemical features.

Six regression models are compared: Ridge, Random Forest, Extra Trees, Gradient Boosting, Hist Gradient Boosting, and XGBoost. Model performance is evaluated using R², MAE, and RMSE. Pearson correlation, prediction plots, residual analysis, and SHAP are used to interpret the results.

## Files

- `machine_learning.ipynb` — Jupyter Notebook for data analysis and modeling.
- `GCD_Future20_ML_ready.xlsx` — input dataset (sheet: `ML_Labeled`), if provided.
- `Figures/` — generated plots, if included.
- `Tables/` — model results, if included.

## How to Run

1. Install Python and Jupyter Notebook (or use VS Code).
2. Install the required packages:

   ```bash
   pip install numpy pandas matplotlib scipy scikit-learn xgboost shap openpyxl joblib
   ```

3. Place the input Excel file in the project folder.
4. Open `machine_learning.ipynb` and run the cells in order.

## Data Note

Please consult the accompanying research manuscript for the data-generation and validation procedures. 

## Research Use

This repository is intended to support research transparency and reproducibility. Please cite the associated publication when using this work.
