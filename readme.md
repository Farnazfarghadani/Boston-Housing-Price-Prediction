## Boston Housing Price Prediction

This project explores the Boston Housing dataset to predict the median value of homes using various regression techniques. After exploratory analysis and model comparison, a **Random Forest Regressor** was selected as the best-performing model.

---

##  Dataset

- **Source**: [Kaggle - Boston Housing Dataset](https://www.kaggle.com/datasets/altavish/boston-housing-dataset)
- **Target Variable**: `MEDV` — Median value of owner-occupied homes (in $1000s)

---

## Features Overview

| Feature | Description |
|---------|-------------|
| CRIM | Per capita crime rate by town |
| ZN | Proportion of residential land zoned for large lots |
| INDUS | Proportion of non-retail business acres per town |
| CHAS | Charles River dummy variable (= 1 if tract bounds river; 0 otherwise) |
| NOX | Nitric oxide concentration (parts per 10 million) |
| RM | Average number of rooms per dwelling |
| AGE | Proportion of owner-occupied units built before 1940 |
| DIS | Weighted distances to employment centers |
| RAD | Index of accessibility to radial highways |
| TAX | Property-tax rate per $10,000 |
| PTRATIO | Pupil–teacher ratio by town |
| B | Proportion of Black residents |
| LSTAT | % lower status of the population |
| **MEDV** | **Target: Median value of homes in $1000s** |

---

## Key Steps

- Performed EDA to explore relationships and detect skewness
- Applied log transformations where appropriate (rm, lstat)
- Scaled features and handled outliers
- Trained multiple models: Linear Regression, Decision Tree, Random Forest
- Tuned hyperparameters using grid search
- Evaluated models using MSE and RMSE
-Chose the best model as the final model

---

## Results

- **Best Model**: Random Forest Regressor
- **MSE**: 0.22
- **RMSE**: ≈ **$460** error in predicting home value

---

##  How to Run

1. Clone the repo:
   ```bash
   git clone https://github.com/FarnazFarghadani/boston-housing-prediction.git
   cd boston-housing-prediction
