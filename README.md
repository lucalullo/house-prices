
# House Prices

**0.12676 Kaggle score - predicting residential property prices with Ridge Regression, feature engineering, and regularized linear modeling.**

This project explores an end-to-end machine learning workflow, from exploratory data analysis and feature preprocessing to hyperparameter tuning and house price prediction.

[![Kaggle Competition](https://img.shields.io/badge/Kaggle-Competition-20BEFF?logo=kaggle&logoColor=white)](https://www.kaggle.com/code/lucalullo/house-prices)
![Kaggle Score](https://img.shields.io/badge/Kaggle_Score-0.12676-2E8B57)
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)
![pandas](https://img.shields.io/badge/pandas-Data_Processing-150458?logo=pandas&logoColor=white)
![scikit-learn](https://img.shields.io/badge/scikit--learn-Ridge_Regression-F7931E?logo=scikitlearn&logoColor=white)

**[View the original Kaggle notebook](https://www.kaggle.com/code/lucalullo/house-prices)** | **[Explore the notebook](house-prices.ipynb)** | **[Author's GitHub](https://github.com/lucalullo)**

---

## At a glance

| | |
|---|---|
| **Task** | Regression: predicting residential property sale prices |
| **Competition** | Kaggle House Prices |
| **Reported score** | **0.12676** |
| **Model** | Ridge Regression with hyperparameter tuning |
| **Feature processing** | Missing value handling, skewness transformations, categorical encoding |
| **Analysis** | Target distribution, feature correlations, exploratory visualizations |
| **Core libraries** | Python, pandas, NumPy, scikit-learn, SciPy, Matplotlib, Seaborn |
| **Environment** | Jupyter Notebook |

## Why this project matters

This project demonstrates how **data preprocessing and feature engineering can support regularized linear regression** in a high-dimensional tabular prediction task.

Rather than relying on a complex ensemble, the workflow focuses on preparing the available features and tuning a Ridge Regression model to predict residential property prices.

The notebook covers:

- **Exploratory data analysis:** examining the target distribution, feature relationships, and correlation patterns.
- **Missing value handling:** applying preprocessing decisions based on the meaning and context of individual features.
- **Numerical transformations:** using Box-Cox and logarithmic transformations to address skewed distributions.
- **Categorical encoding:** converting categorical information, including quality-related features, into model-compatible representations.
- **Regularized regression:** applying Ridge Regression to control model complexity in a dataset with numerous features.
- **Hyperparameter tuning:** adjusting the model's regularization settings to improve predictive performance.

## Approach

```text
House price dataset
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
Categorical feature encoding
        |
        v
Ridge Regression
        |
        v
Hyperparameter tuning
        |
        v
House price predictions
```

### Implementation details

| Component | Approach |
|---|---|
| Exploratory analysis | Target distribution visualizations and correlation matrices |
| Missing values | Feature-specific imputation and preprocessing |
| Numerical features | Box-Cox transformations and logarithmic scaling |
| Categorical features | Encoding of categorical and quality-related variables |
| Regression model | Ridge Regression with L2 regularization |
| Model optimization | Hyperparameter tuning |
| Evaluation | Reported Kaggle competition score |

The workflow emphasizes the role of preprocessing in making a regularized linear model suitable for structured housing data.

## Competition result

> **Reported Kaggle score: 0.12676.**

The score is reported for the Ridge Regression approach described in the original project.

It should not be interpreted as evidence that Ridge Regression outperforms other regression algorithms. No systematic comparison against alternative models is documented here.

[Explore the original Kaggle notebook](https://www.kaggle.com/code/lucalullo/house-prices).

## Repository contents

```text
House-price/
├── README.md
└── house-prices.ipynb
```

The notebook contains the project's exploratory analysis, preprocessing steps, and regression modeling workflow.

## Run the notebook

The original project is available on **Kaggle**, where the notebook can be explored in its competition environment.

To run the project locally, install the required Python libraries:

```bash
python -m pip install pandas numpy seaborn matplotlib scikit-learn scipy jupyter
```

Then open `house-prices.ipynb` in Jupyter.

The relevant Kaggle competition data must be available, and any dataset paths used in the notebook may need to be adjusted for the local environment.

## Scope and limitations

- The project focuses on **Ridge Regression**, rather than a systematic benchmark of multiple regression algorithms.
- Model performance depends on the preprocessing decisions and the selected regularization settings.
- Numerical transformations and categorical encoding are tailored to the available housing features.
- The reported Kaggle score reflects competition performance and does not establish generalization to different housing markets or datasets.
- Reproducing the original results requires the relevant competition data and compatible preprocessing steps.

## Related work

This project complements my other work on applied machine learning, tabular data analysis, and predictive modeling with Python.

- [GitHub profile and selected projects](https://github.com/lucalullo)
- [Kaggle profile](https://www.kaggle.com/lucalullo)

---

**Author:** [Luca Lullo](https://github.com/lucalullo)  
**Original project:** [House Prices - Kaggle](https://www.kaggle.com/code/lucalullo/house-prices)
