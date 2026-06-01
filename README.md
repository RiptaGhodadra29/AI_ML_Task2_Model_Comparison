# AI_ML_Task2_Model_Comparison
# Feature Engineering, Model Optimization & Performance Comparison

## Project Overview

This project focuses on predicting California housing prices using Machine Learning regression models. The objective is to perform feature engineering, data preprocessing, feature scaling, model training, model optimization, and performance comparison to identify the best-performing model.

The California Housing Dataset from Scikit-Learn was used for this project. Multiple regression algorithms were trained and evaluated using standard performance metrics.

---

## Objective

The objectives of this project are:

* Load and explore the California Housing Dataset.
* Perform data preprocessing and feature engineering.
* Apply feature scaling using StandardScaler.
* Train multiple regression models.
* Compare model performance.
* Evaluate models using RMSE and R² Score.
* Select the best-performing model.

---

## Dataset Information

Dataset: California Housing Dataset

Source:

```python
from sklearn.datasets import fetch_california_housing
```

### Features

* MedInc → Median Income
* HouseAge → Median House Age
* AveRooms → Average Rooms
* AveBedrms → Average Bedrooms
* Population → Population
* AveOccup → Average Occupancy
* Latitude → Latitude
* Longitude → Longitude

### Target Variable

* HousePrice (Median House Value)

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-Learn
* Jupyter Notebook

---

## Project Workflow

### 1. Data Collection

The California Housing Dataset was loaded directly from Scikit-Learn.

### 2. Data Exploration

Performed:

* Dataset Shape Analysis
* Data Type Inspection
* Statistical Summary
* Missing Value Analysis

### 3. Feature Engineering & Preprocessing

* Feature Selection
* Target Variable Selection
* Train-Test Split
* Feature Scaling using StandardScaler

### 4. Model Training

The following regression algorithms were implemented:

#### Linear Regression

A basic regression algorithm that models a linear relationship between input features and the target variable.

#### Ridge Regression

An improved version of Linear Regression that includes L2 regularization to reduce overfitting.

#### Decision Tree Regressor

A tree-based model capable of capturing non-linear relationships within the dataset.

---

## Evaluation Metrics

The following metrics were used to evaluate model performance:

### RMSE (Root Mean Squared Error)

Measures prediction error.

* Lower RMSE = Better Model

### R² Score (Coefficient of Determination)

Measures how well the model explains the variance in the target variable.

* Higher R² Score = Better Model

---

## Model Performance Comparison

| Model                   | RMSE     | R² Score |
| ----------------------- | -------- | -------- |
| Linear Regression       | 0.745581 | 0.575788 |
| Ridge Regression        | 0.745557 | 0.575816 |
| Decision Tree Regressor | 0.724234 | 0.599732 |

---

## Model Ranking

| Rank | Model                   | RMSE     | R² Score |
| ---- | ----------------------- | -------- | -------- |
| 1    | Decision Tree Regressor | 0.724234 | 0.599732 |
| 2    | Ridge Regression        | 0.745557 | 0.575816 |
| 3    | Linear Regression       | 0.745581 | 0.575788 |

---

## Result Analysis

### Linear Regression

* RMSE: 0.745581
* R² Score: 0.575788

Linear Regression provided a solid baseline performance but was limited in capturing complex non-linear relationships in the housing data.

### Ridge Regression

* RMSE: 0.745557
* R² Score: 0.575816

Ridge Regression slightly outperformed Linear Regression due to regularization, helping reduce overfitting.

### Decision Tree Regressor

* RMSE: 0.724234
* R² Score: 0.599732

Decision Tree Regressor achieved the best performance among all tested models. It successfully captured non-linear patterns present in the dataset, resulting in improved prediction accuracy.

---

## Best Model

### Decision Tree Regressor

Performance:

* RMSE = 0.724234
* R² Score = 0.599732

Reason for Selection:

* Lowest prediction error
* Highest explanatory power
* Best overall performance among all evaluated models

---


## Conclusion

This project successfully implemented the complete Machine Learning workflow, including data preprocessing, feature scaling, model training, model evaluation, and performance comparison.

Three regression algorithms were evaluated:

* Linear Regression
* Ridge Regression
* Decision Tree Regressor

The models were assessed using RMSE and R² Score. Among all models, the Decision Tree Regressor achieved the best performance with an RMSE of 0.724234 and an R² Score of 0.599732.

The results demonstrate that tree-based models can effectively capture complex and non-linear relationships in housing datasets, leading to better prediction accuracy than traditional linear models.

Therefore, the Decision Tree Regressor was selected as the final model for California housing price prediction.

---




---

## Requirements

```text
numpy
pandas
matplotlib
seaborn
scikit-learn
joblib
```

---



AI & Machine Learning Internship Task 2

Feature Engineering, Model Optimization & Performance Comparison
