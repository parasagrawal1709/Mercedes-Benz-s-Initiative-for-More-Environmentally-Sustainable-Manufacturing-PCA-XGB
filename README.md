# Mercedes-Benz Environmentally Sustainable Manufacturing: Machine Learning Model to Minimize Vehicle Testing Duration

## Table of Contents

- [Introduction](#introduction)
- [Motivation & Aim](#motivation--aim)
- [Problem Statement](#problem-statement)
- [Tasks Performed](#tasks-performed)
- [Data Preparation](#data-preparation)
- [Feature Engineering](#feature-engineering)
- [Model Building](#model-building)
- [Results and Evaluation](#results-and-evaluation)

## Introduction

This project focuses on developing a machine learning model to optimize the testing duration of Mercedes-Benz vehicles by leveraging advanced data preprocessing techniques and predictive algorithms. The goal is to ensure that the vehicle testing process is both efficient and environmentally sustainable by minimizing unnecessary time spent on the test bench.

## Motivation & Aim

The aim of this project is to minimize the duration of Mercedes-Benz vehicles undergoing testing. By optimizing the testing process, Mercedes-Benz can achieve a more environmentally sustainable manufacturing process while maintaining the highest standards of safety and reliability for its customers.

## Problem Statement

Mercedes-Benz is a leader in automotive innovation, with a strong focus on safety, efficiency, and sustainability. The company offers numerous vehicle features and options, resulting in a wide range of car configurations. To ensure the safety and reliability of every car configuration, a robust testing framework is necessary. However, this testing process is time-consuming due to the large number of potential feature combinations. This project aims to streamline the testing process by utilizing sophisticated algorithmic solutions.

## Tasks Performed

1. **Data Cleaning**: Removed columns with zero variance.
2. **Data Exploration**: Checked for null and unique values in the datasets.
3. **Label Encoding**: Applied label encoding to categorical features.
4. **Dimensionality Reduction**: Performed Principal Component Analysis (PCA) to reduce dimensionality.
5. **Model Building**: Built a predictive model using XGBoost to make predictions on the test dataset.

## Data Preparation

- **Data Loading**: Loaded the training and test datasets using `pandas`.
- **EDA (Exploratory Data Analysis)**: Analyzed the data to understand its structure, missing values, and unique values.
- **Data Cleaning**: Identified and removed columns with zero variance to improve model performance.
- **Label Encoding**: Encoded categorical features using a custom label encoder to handle unknown labels.

## Feature Engineering

- **Dimensionality Reduction**: Used PCA to reduce the feature space while retaining 94% of the variance with the first 5 principal components.
- **Data Preprocessing**: Scaled numeric features and applied one-hot encoding for categorical features.

## Model Building

- **Algorithm Used**: XGBoost regressor.
- **Model Training**: Trained the model using a training dataset split into training and validation sets.
- **Hyperparameter Tuning**: Set parameters such as learning rate (`eta`), maximum depth, and the number of boosting rounds.
- **Prediction**: Made predictions on the test dataset using the trained XGBoost model.

## Results and Evaluation

- **R-squared Score**: Calculated the R-squared score for both training and validation datasets.
- **RMSE**: Computed the Root Mean Square Error (RMSE) for training and validation datasets.
