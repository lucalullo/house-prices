
# House Prices

**0.12676 Kaggle competition score - predicting residential property prices with Ridge Regression, feature engineering, and regularized linear modeling.**

This project explores an end-to-end machine learning workflow, from exploratory data analysis and feature preprocessing to hyperparameter tuning and house price prediction.

[![Kaggle Competition](https://img.shields.io/badge/Kaggle-Competition-20BEFF?logo=kaggle&logoColor=white)](https://www.kaggle.com/code/lucalullo/house-prices)
![Kaggle Score](https://img.shields.io/badge/Kaggle_Score-0.12676-2E8B57)
![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-Data_Processing-150458?logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-Ridge_Regression-F7931E?logo=scikitlearn&logoColor=white)

**[View the original Kaggle notebook](https://www.kaggle.com/code/lucalullo/house-prices)** | **[Explore the notebook](house-prices.ipynb)** | **[Author's GitHub](https://github.com/lucalullo)**

---

## At a glance

| | |
|---|---|
| **Task** | Regression: residential property sale price prediction |
| **Competition** | Kaggle House Prices |
| **Reported score** | **0.12676** |
| **Model** | Ridge Regression with hyperparameter tuning |
| **Feature processing** | Missing value handling, numerical transformations, categorical encoding |
| **Analysis** | Target distribution, feature correlations, exploratory visualizations |
| **Core libraries** | pandas, NumPy, scikit-learn, SciPy, Matplotlib, Seaborn |
| **Environment** | Python and Jupyter Notebook |

## Why this project matters

This is a **feature-engineering-focused machine learning experiment**: the emphasis is on preparing structured housing data and applying regularized linear regression to a prediction task involving numerous numerical and categorical features.

The notebook covers:

- **Exploratory data analysis:** visualizing the target distribution and examining correlations between features.
- **Missing value handling:** applying preprocessing decisions based on individual feature characteristics.
- **Numerical transformations:** using Box-Cox and logarithmic transformations to address skewed distributions.
- **Categorical encoding:** preparing categorical and quality-related features for regression modeling.
- **Regularized regression:** using Ridge Regression to control model complexity and reduce overfitting.
- **Hyperparameter tuning:** optimizing model settings for predictive performance.

## Approach

```text
Kaggle housing data
        |
        v
Exploratory data analysis
        |
        v
Missing value handling
        |
        v
Numerical transformations
        |
        v
Categorical encoding
        |
        v
Ridge Regression + hyperparameter tuning
        |
        v
House price predictions
```

### Implementation details

| Component | Notebook approach |
|---|---|
| Exploratory analysis | Target distribution and correlation matrices |
| Missing values | Feature-specific preprocessing |
| Numerical features | Box-Cox and logarithmic transformations |
| Categorical features | Encoding of categorical and quality-related variables |
| Model | Ridge Regression with L2 regularization |
| Model selection | Hyperparameter tuning |
| Evaluation | Reported Kaggle competition score |

The notebook focuses on a regularized linear regression approach rather than a systematic comparison of multiple predictive models.

## Competition result

> **Kaggle score: 0.12676.**

This is the competition score reported for the original Ridge Regression solution.

It is **not** presented as a benchmark proving superiority over other regression algorithms; no systematic comparative benchmark is provided here.

[See the original Kaggle notebook](https://www.kaggle.com/code/lucalullo/house-prices).

## Repository contents

```text
House-price/
├── README.md
└── house-prices.ipynb
```

The notebook contains the original exploratory analysis, preprocessing workflow, and regression modeling.

## Run the notebook

The reference environment is **Kaggle**, where the original notebook is available.

To run it locally, install the required dependencies:

```bash
python -m pip install pandas numpy seaborn matplotlib scikit-learn scipy jupyter
```

Then open `house-prices.ipynb` in Jupyter and make the Kaggle competition data available.

**Local execution may require updating dataset paths inside the notebook** to match the location of the downloaded files.

## Scope and limitations

- The project focuses on **Ridge Regression** rather than a systematic comparison of regression algorithms.
- Preprocessing decisions and numerical transformations are tailored to the competition dataset.
- The reported competition score does not establish performance on unrelated housing markets or datasets.
- Reproducing the results requires access to the relevant Kaggle competition data.
- The original project description does not document a separate external validation study.

## Related work

This project complements my other work on applied machine learning, feature engineering, and reproducible data analysis.

- [GitHub profile and selected projects](https://github.com/lucalullo)
- [Kaggle profile](https://www.kaggle.com/lucalullo)

---

**Author:** [Luca Lullo](https://github.com/lucalullo)  
**Original Kaggle work:** [House Prices](https://www.kaggle.com/code/lucalullo/house-prices)
