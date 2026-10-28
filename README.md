# Machine Learning Project: Insurance Cost Prediction

This is a beginner-level machine learning project that explores how personal and lifestyle factors relate to medical insurance expenses. It uses a public insurance dataset and compares two regression models to estimate a person's insurance expenses from their profile.

## Project overview

The project is implemented as a Jupyter Notebook. It walks through the main stages of a basic machine learning workflow:

1. Load and explore the dataset with summary statistics and visualizations.
2. Prepare categorical features using one-hot encoding and binary encoding.
3. Split the data into training and test sets (80% / 20%).
4. Standardize features for Linear Regression.
5. Train and compare Linear Regression and Random Forest Regressor.
6. Evaluate predictions with MAE, RMSE, and R², and inspect feature importance and residuals.
7. Generate example predictions for a new customer profile.

The target column is `expenses`. Input features are age, sex, BMI, number of children, smoking status, and region.

## Technologies

- Python
- Jupyter Notebook
- pandas and NumPy for data handling
- Matplotlib and Seaborn for visualizations
- scikit-learn for preprocessing, model training, and evaluation

## Getting started

### Requirements

Python 3.9 or newer is recommended.

### Install dependencies

```bash
python -m pip install -r requirements.txt
```

### Run the notebook

Keep `insurance.csv` in the repository root and launch Jupyter from that directory so the notebook can find the dataset:

```bash
jupyter notebook
```

Then open `ML_Insurance_Cost_Prediction/Insurance_Cost_Prediction.ipynb` and run the cells from top to bottom.

## Example results

The notebook's saved results show the following scores on its 20% test split:

| Model | MAE | RMSE | R² |
| --- | ---: | ---: | ---: |
| Linear Regression | 4,181.56 | 5,796.56 | 0.7836 |
| Random Forest Regressor | 2,548.50 | 4,570.97 | 0.8654 |

On this split, Random Forest performs better. These results are for learning and demonstration; they do not establish that the model is suitable for real insurance pricing or financial decisions.

## Repository structure

```text
.
├── insurance.csv
├── README.md
├── requirements.txt
└── ML_Insurance_Cost_Prediction/
    └── Insurance_Cost_Prediction.ipynb
```

## Dataset

The notebook uses the `insurance.csv` dataset included in this repository. If you redistribute the data, retain any attribution or license terms supplied with its original source.

