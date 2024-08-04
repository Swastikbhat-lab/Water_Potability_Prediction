# Drinking Water Potability Prediction

This project aims to predict the potability of drinking water using various machine learning models. The dataset contains various water quality parameters, and the goal is to classify the water as potable or not.

## Table of Contents
- [Project Overview](#project-overview)
- [Tech Stack](#tech-stack)
- [AI Models](#ai-models)
- [Data Preprocessing](#data-preprocessing)
- [Model Training and Evaluation](#model-training-and-evaluation)
- [Usage](#usage)
- [Results](#results)
- [Contributing](#contributing)

## Project Overview
The project utilizes machine learning models to classify water samples based on their potability. It involves data preprocessing, model selection, and evaluation. The project leverages H2O.ai's AutoML framework for model training and evaluation.

## Tech Stack
- **Programming Language**: Python
- **Libraries**: 
  - `pandas`: Data manipulation and analysis
  - `numpy`: Numerical computations
  - `matplotlib` & `seaborn`: Data visualization
  - `sklearn`: Machine learning utilities
  - `H2O.ai`: AutoML for model selection and evaluation

## AI Models
The project uses the H2O.ai AutoML framework to automatically train and tune a variety of machine learning models. The following models were considered:
- **GLM** (Generalized Linear Model)
- **GBM** (Gradient Boosting Machine)
- **XGBoost** (Extreme Gradient Boosting)
- **Random Forest**
- **Deep Learning** models

The best-performing model, according to the AutoML leaderboard, was a Stacked Ensemble model, which combines multiple models for better performance.

## Data Preprocessing
The dataset is preprocessed by handling missing values, feature scaling, and encoding categorical variables. Feature engineering steps include:
- Imputation of missing values
- Scaling numerical features
- Encoding categorical variables, if any

## Model Training and Evaluation
The H2O.ai AutoML framework was used to train and evaluate multiple models. The process involves:
- Splitting the dataset into training and testing sets
- Training multiple models using AutoML
- Evaluating models based on accuracy, AUC, and other metrics
- Selecting the best model based on performance metrics

## Usage
To use the model for predictions, follow these steps:
1. Load the dataset and preprocess it as per the preprocessing steps mentioned.
2. Use the trained model (`aml.leader`) to make predictions on new data.

Example:
```python
y_pred = aml.leader.predict(df_test)
