# Spaceship titanic

**Kaggle dataset:** [Dataset](https://www.kaggle.com/competitions/spaceship-titanic)

## Objective

The goal of this project is to predict whether a passenger was transported to an alternate dimension during the Spaceship Titanic's collision with a spacetime anomaly. (binary classification)

Additionally, this was project marks my introduction to concrete statistical analysis before feature engineering. (Hypothesis testing, p-values etc)

## Data Overview
* **Source:** `Kaggle`
* **Key Feature:** `CryoSleep` 
* **Target Variable:** `Transported`

## Methodology & Models

In this notebook, I performed imputation based on domain knowledge, imputing Cryosleep status from passenger spending patters, and HomePlanet from shared group_id.

Upon plotting histograms for continuous values and bar charts for categorical ones, I visually confirmed suspicions such as, spending being right-skewed (passengers with 0 spend on cryosleep and dominating spending by the top few), Age not having a normal distribution, having centres around ages 0-5 and again around 20-25.
I used chi-square tests of independence and Mann-Whitney U tests (with effect sizes (Cramer's V and Rank Biserial)) to validate feature relationships with the target variable before modelling.

The mdoels trained in this notebook are, `XGBoost`, and `Random Forest`.

## Results (Test set)
| Model | Accuracy | 
|---|---|
| **XGBoost** | **80.19%** |
| Random Forest | *79.2%* |
