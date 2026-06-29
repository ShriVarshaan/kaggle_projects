# Bank Customer Churn Prediction

**Kaggle Dataset:** [dataset](https://www.kaggle.com/datasets/shrutimechlearn/churn-modelling/data)

##  Objective

"The goal of this project is to predict whether a bank customer will close their account (churn) based on demographic and financial data."

## Data Overview
* **Source:** Kaggle
* **Target Variable:** `Exited`
* **Key Features:** `Geography, Credit Score and Age`

## Methodology & Models
In this notebook, I performed data preprocessing (handling missing values, encoding categorical variables, and scaling) before training and evaluating the following three models:

1. **XGBoost**
2. **XGBoost -- Tuned hyperparameters**
3. **Model 3 Name, Random Forest**
4. **Model 4 Name, e.g., Random Forest -- Tuned hyperparameters**

##  Results (Validation set)
| Model | Accuracy | F1-Score |
|---|---|---|
| XGBoost | 81% | 0.63 |
| XGBoost Tuned | 83.8% | 0.65 |
| Random Forest | 80.2% | 0.63 |
| **Random Forest Tuned (Best)** | **85%** | **0.65** |

##  Results (Test set)
| Model | Accuracy | F1-Score |
|---|---|---|
| **Random Forest Tuned (Best)** | **84.8%** | **0.63** |
