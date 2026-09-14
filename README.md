# Medical Insurance Cost Prediction using Machine Learning

## Project Overview

This project focuses on predicting medical insurance charges using Machine Learning.

The model uses customer-related information such as age, sex, BMI, number of children, smoking status, and region to predict medical insurance charges.

## Problem Statement

The objective of this project is to build a regression model that can predict medical insurance costs based on different customer characteristics.

## Dataset

The dataset contains the following features:

- Age
- Sex
- BMI
- Number of children
- Smoking status
- Region
- Medical insurance charges

The target variable is `charges`.

## Technologies Used

- Python
- Pandas
- Seaborn
- Scikit-learn
- Jupyter Notebook

## Machine Learning Workflow

1. Loaded the dataset using Pandas.
2. Explored the dataset and checked for missing values.
3. Visualized the relationship between BMI, smoking status, and insurance charges.
4. Separated features and target variable.
5. Converted categorical variables into numerical form.
6. Applied One-Hot Encoding to the `region` feature.
7. Created interaction features such as `age × smoker` and `bmi × smoker`.
8. Split the dataset into training and testing sets.
9. Trained a Linear Regression model.
10. Generated predictions on the test dataset.
11. Evaluated the model using R² and Adjusted R².
12. Compared training and testing performance to analyze model generalization.

## Feature Engineering

Two interaction features were created:

- `age_smoker = age × smoker`
- `bmi_smoker = bmi × smoker`

These features were created to capture the combined effect of age and BMI with smoking status.

## Model Evaluation

The model was evaluated using:

- R² Score
- Adjusted R²
- Training vs Testing R² comparison

The training and testing scores were compared to understand whether the model was underfitting or overfitting.

## Project Structure

```text
Medical-Insurance-Cost-Prediction/
│
├── insurance.csv
├── medical_insurance_cost_prediction.ipynb
└── README.md

## Conclusion

This project demonstrates a basic end-to-end Machine Learning regression workflow, including data preprocessing, categorical encoding, feature engineering, model training, prediction, and model evaluation using Linear Regression.
