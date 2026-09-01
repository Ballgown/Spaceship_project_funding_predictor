# Spaceship-project-funding-predictor

An end-to-end Machine Learning web application engineered to predict capital budget allocations and funding requirements for aerospace mission prototypes. The solution integrates an optimized Random Forest Regression pipeline, comprehensive exploratory data analysis, and an interactive Flask deployment framework for real-time inference.

# Executive Summary

Estimating technical budget requirements for multi-stage engineering initiatives involves navigating non-linear feature interactions, depreciation vectors, historical expenditure trends, and capacity parameters.

This repository provides an automated inference pipeline that:

Cleanses, standardizes, and encodes multi-variable prototype parameters.

Trains an ensemble RandomForestRegressor with hyperparameter optimization.

Serves low-latency predictions via an interactive web dashboard.

# Architecture Pipeline

Raw Data (CSV) -> Preprocessing and EDA -> Feature Encoding -> Random Forest Regressor Pipeline -> Model Serialization (.pkl) -> Flask REST Engine / UI Layer -> Real-Time Valuation

# Key Technical Highlights

Automated Data Processing: Systematic handling of numerical variance, missing values, and categorical one-hot encoding across engineering attributes.

Non-Linear Regression Modeling: Mitigates overfitting through bootstrap aggregation and tree-depth regularization.

Low-Latency Inference Engine: Pickled pipeline serving predictions in sub-100ms response times.

Responsive Frontend Dashboard: Built using HTML5, CSS3, and Jinja2 templating for intuitive parameter manipulation.

# Tech Stack and Dependencies

Core Engine: Python 3.x

Data Science and ML: pandas, numpy, scikit-learn, joblib

Web Server: Flask, gunicorn, Jinja2

Visualization (Exploratory Phase): seaborn, matplotlib

# Evaluation and Metrics

The regression model optimizes against primary statistical criteria:

Coefficient of Determination (R2 Score): Measures variance explained by the ensemble architecture.

Mean Absolute Error (MAE): Quantifies average absolute divergence in estimated capital.

Root Mean Squared Error (RMSE): Penalizes significant outlier deviations in projection scales.
