# ML CHALLENGE

This repository contains a machine learning project built for a data challenge. It manages the entire workflow, from exploratory data analysis to data preparation, model training, and submission generation.

## Project Structure

- `data/`
  - `raw/`: Raw datasets, including training, validation, and test files.
- `notebooks/`
  - `01_data_audit.ipynb`: Initial data audit.
  - `02_eda.ipynb`: Exploratory Data Analysis (EDA).
  - `03_feature_engineering.ipynb`: Feature engineering and transformations.
  - `04_lightgbm.ipynb`: Training and evaluation of a LightGBM model.
  - `05_catboost.ipynb`: Training and evaluation of a CatBoost model.
  - `06_ensemble.ipynb`: Building an ensemble model.
- `src/`
  - `preprocessing.py`: Data preprocessing functions.
  - `features.py`: Feature generation functions.
  - `train_lightgbm.py`: LightGBM training script.
  - `train_catboost.py`: CatBoost training script.
  - `predict.py`: Prediction and submission file generation script.
- `models/`
  - `catboost/`, `lightgbm/`, `ensemble/`: Saved models or output directories.
- `submission/`
  - Generated submission files.
- `notes/` and `reports/`: Documentation of experiments, hypotheses, and visualizations.

## Objective

The goal is to develop a robust solution for a machine learning challenge by:

1. Exploring and auditing the data.
2. Cleaning and preparing the datasets.
3. Building relevant features (Feature Engineering).
4. Training multiple models (LightGBM, CatBoost, ensemble).
5. Generating final predictions for submission.

## Usage

1. Install the dependencies:

```bash
pip install -r requirements.txt
