# SWYNEX Data Preparation - House Prices Dataset

## Overview
This project prepares the [House Prices - Advanced Regression Techniques](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques) dataset (Ames, Iowa housing data) for machine learning, as part of the SWYNEX Data Science internship (Task 1).

## Dataset
- **Source:** Kaggle competition dataset
- **Size:** 1,460 rows × 81 columns
- **Target variable:** SalePrice

## Steps Performed
1. **Exploratory Data Analysis** — checked shape, data types, and missing values
2. **Missing Value Handling** — referenced `data_description.txt` to distinguish between genuinely missing data and NaN values that mean "feature doesn't exist" (e.g., no pool, no garage)
3. **Type Fixing** — ensured all columns had appropriate data types
4. **Ordinal Encoding** — mapped quality/condition columns (e.g., Poor→Excellent) to numeric scales that preserve order
5. **Nominal Encoding** — one-hot encoded remaining categorical columns with no inherent order
6. **Feature/Target Split** — separated features (X) from the target variable (y)

## Result
Final dataset: 1,460 rows × 205 features, fully numeric with zero missing values, ready for model training.

## How to Run
1. Clone this repo
2. Install dependencies: `pip install pandas numpy`
3. Place `train.csv` in the project folder
4. Run `data_preparation.ipynb`

## Files
- `data_preparation.ipynb` — main notebook with all preprocessing steps
- `README.md` — this file
