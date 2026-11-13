# House Prices

**Residential sale price prediction with feature preprocessing, log-transformed targets, and Ridge Regression.**

This Kaggle notebook explores the House Prices regression competition, preparing numerical and categorical housing features and fitting a regularized linear model.

![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white) ![scikit-learn](https://img.shields.io/badge/scikit--learn-Ridge_Regression-F7931E?logo=scikitlearn&logoColor=white) [![Kaggle Notebook](https://img.shields.io/badge/Kaggle-Notebook-20BEFF?logo=kaggle&logoColor=white)](https://www.kaggle.com/code/lucalullo/house-prices)

[Kaggle notebook](https://www.kaggle.com/code/lucalullo/house-prices) · [Explore the notebook](house-prices.ipynb) · [GitHub profile](https://github.com/lucalullo)

## At a glance

| | |
|---|---|
| **Task** | Regression: residential sale price (`SalePrice`) |
| **Competition** | Kaggle House Prices: Advanced Regression Techniques |
| **Reported Kaggle score** | **0.12676** (reported in the existing project README; not independently verified from the notebook) |
| **Recorded validation RMSE** | **0.11728** (notebook output, log-transformed target scale) |
| **Model** | Ridge Regression (`alpha=10`) |
| **Validation** | 80/20 train/validation split |
| **Preprocessing** | Missing values, skewed numerical features, one-hot categorical encoding |
| **Core libraries** | pandas, NumPy, scikit-learn, SciPy, Matplotlib, Seaborn |
| **Data** | Kaggle competition train/test CSVs (not redistributed) |

## Project overview

This is an **applied tabular regression experiment** that examines how cleaning, feature transformations, and linear regularization can support house price prediction.

The notebook covers:

- **Exploration:** distributions and correlations in the training data.
- **Preprocessing:** missing-value handling and removal or transformation of selected variables.
- **Target transformation:** fitting the model to `log1p(SalePrice)`.
- **Categorical encoding:** one-hot encoding and train/test feature alignment.
- **Regularized regression:** Ridge Regression with a fixed `alpha=10`.
- **Submission:** fitting on all labeled rows, inverting the log transformation, and creating `submission.csv`.

## Methodology

```text
Kaggle train/test data
        |
        v
Exploratory analysis + cleaning
        |
        v
Numerical transformations
        |
        v
One-hot encoding + column alignment
        |
        v
Log-transformed target
        |
        v
Train/validation split
        |
        v
Ridge Regression (alpha=10)
        |
        v
Validation RMSE on log scale
        |
        v
Refit on all labeled rows
        |
        v
Inverse transform -> submission.csv
```

### Implementation details

| Component | Notebook implementation |
|---|---|
| Target | `np.log1p(SalePrice)` |
| Categorical variables | `pd.get_dummies`, followed by train/test column alignment |
| Validation | `train_test_split(test_size=0.2, random_state=42)` |
| Estimator | `Ridge(alpha=10)` |
| Validation metric | RMSE calculated on log-transformed predictions and targets |
| Output | `np.expm1` converts predictions back to sale prices |

The notebook uses a **fixed Ridge regularization parameter**. It does not contain an automated hyperparameter search or model comparison.

## Results

> **Recorded holdout RMSE: 0.11728** on the log-transformed target scale.

The previous project README also reports a **Kaggle competition score of 0.12676**. That score is retained as a reported competition result, but the archived notebook does not independently establish its leaderboard provenance. The holdout result and Kaggle score should not be presented as interchangeable measurements.

## Repository structure

```text
house-prices/
├── README.md
├── house-prices.ipynb
├── .gitignore
└── LICENSE
```

## Getting started

The reference environment is **Kaggle**. The notebook reads competition data from:

```text
/kaggle/input/competitions/house-prices-advanced-regression-techniques/
```

For local execution, install the principal notebook dependencies:

```bash
python -m pip install pandas numpy scipy scikit-learn matplotlib seaborn jupyter
```

Download the competition train/test CSVs, open `house-prices.ipynb`, and replace the Kaggle-specific file paths with local paths. The notebook generates `submission.csv`.

## Limitations

- The model uses a single Ridge configuration rather than automated tuning or comparison with nonlinear estimators.
- The validation result comes from one holdout split; no cross-validation is shown.
- The Kaggle score comes from the original project description, not a documented leaderboard artifact inside the notebook.
- Performance outside the competition housing dataset is unknown.
- The competition data are not redistributed; access and permitted use are governed by Kaggle.

## Related work

- [GitHub profile and selected projects](https://github.com/lucalullo)
- [Kaggle profile](https://www.kaggle.com/lucalullo)

## Author

Created by [Luca Lullo](https://github.com/lucalullo). Original work: [House Prices on Kaggle](https://www.kaggle.com/code/lucalullo/house-prices).
