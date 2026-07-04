# IMDB movie review sentiment analysis

**Kaggle dataset:** [Dataset](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews)

## Objective

The goal of this project is to predict whether a given movie review is positive or negative. (sentiment analysis)

## Data Overview
* **Source:** Kaggle
* **Target Variable:** sentiment

## Methodology & Models
In this notebook, I performed feature hashing to convert the texts to integers using keras' one_hot function. Models trained in this notebook are

1. **Simple RNN model**

## Results (Test set)
| Model | Accuracy | Precision | Recall |
|---|---|---|---|
| Simple RNN | 82.77% | 0.8206 | 0.8422 |
