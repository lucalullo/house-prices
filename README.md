# House Prices

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Kaggle](https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=Kaggle&logoColor=white)

This repository contains a comprehensive data science workflow for predicting residential home prices. 

🔗 **Original Notebook on Kaggle:** [View here](https://www.kaggle.com/code/lucalullo/house-prices)

## 📈 Performance
- **Kaggle Score (RMSE):** 0.12676
- **Model:** Ridge Regression with hyperparameter tuning.

## 🛠️ Key Features
- **Exploratory Data Analysis (EDA):** Detailed visualization of target distribution and correlation matrices.
- **Advanced Preprocessing:** - Handling missing values based on feature context.
  - **Box-Cox transformation** and Log-scaling for skewed numerical features.
  - Categorical encoding for quality-related features.
- **Modeling:** Implementation of Regularized Linear Models (Ridge) to prevent overfitting given the high number of features (79+).

## 🚀 How to use
1. Clone the repo: `git clone https://github.com/lucalullo/House-price.git`
2. Install dependencies: `pip install pandas numpy seaborn matplotlib scikit-learn scipy`
3. Run the `house-prices.ipynb` notebook.

---
**Author:** [Luca Lullo](https://github.com/lucalullo)  
*Data Scientist | Machine Learning Applied*
