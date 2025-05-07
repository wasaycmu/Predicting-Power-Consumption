# Electricity Consumption Prediction in Dallas, Texas

## Overview

This project focuses on determining the best method to predict electricity consumption in Dallas, Texas using various machine learning models. The goal is to accurately predict electricity usage, promote energy savings, and provide actionable insights for consumers in the southern United States, specifically Texas.

### Institution:  
Southern Methodist University, Dallas, TX

## Abstract

This project investigates the effectiveness of different machine learning and artificial intelligence models in predicting electricity usage in Dallas, Texas. We aim to bridge the gap in electricity consumption prediction research, which has predominantly focused on European and Eastern Asian demographics, by applying these methods to the US market. By synthesizing datasets that account for regional climate, housing characteristics, and demographics, we seek to achieve the same level of prediction accuracy as previous research.

### Keywords
- Electricity Prediction
- Linear Regression
- Support Vector Regression
- Extreme Gradient Boosting (XGBoost)
- Random Forest
- Neural Networks
- Direct Load Monitoring (DLM)
- Non-Intrusive Load Monitoring (NILM)
- Mean Squared Error (MSE)
- R-squared (R²)

## Motivation

Increased awareness of electricity consumption has been shown to significantly reduce energy use. Studies suggest that informed consumers can save up to 40% on their energy bills, with a 25% average savings. This project leverages machine learning to predict electricity consumption and help consumers reduce costs and their carbon footprint.

## Related Work

Numerous studies have used machine learning to predict electricity consumption globally. Our project builds on these works, including methods such as:
- **Recurrent Neural Networks (RNNs)**
- **Stacking Models** combining multiple algorithms
- **Ensemble Neural Networks** for better prediction accuracy

We aim to apply these techniques to US-specific data, focusing on the southern United States' climate, housing types, and demographics, which may differ significantly from other regions.

## Methods

### Data Collection

The dataset includes:
1. **Metadata Subsection**: System data and participant contact info.
2. **Demographic Information**: Household size, age distribution, etc.
3. **Dwelling Characteristics**: Housing size, construction materials, and orientation.
4. **Appliance Usage Metrics**: Information on appliance types and usage patterns.
5. **Consumption and Pricing Data**: Measured in kWh for standardized comparison.

Due to data privacy concerns, we supplement missing data with synthetic data generated for this study.

### Models

We trained and tested the following machine learning models:
- **Linear Regression** (with and without L2 regularization)
- **Support Vector Regression (SVR)**
- **Extreme Gradient Boosting (XGBoost)**
- **Random Forest**
- **Wide and Deep Neural Networks**

Each model was evaluated based on two metrics: **Mean Squared Error (MSE)** and **R² Coefficient**. We used GridSearchCV for hyperparameter tuning in models such as Linear Regression, SVR, XGBoost, and Random Forest.

### Data Preprocessing

We used an 80/20 training/validation split and applied KFold cross-validation (10 folds) for most models. For neural networks, we experimented with various architectures, including layers with and without Batch Normalization and pre-normalized data.

## Results

- **Linear Regression (L2 Regularized)**: R² = 0.839 (KFold), MSE = 28,219.346
- **Support Vector Regression**: R² = 0.871 (KFold), MSE = 26,480.781
- **XGBoost**: Highest performance with R² = 0.904 (KFold), MSE = 24,369.227

The XGBoost model outperformed others, making it the best choice for this application.

## Conclusion

Our research shows that machine learning models can effectively predict electricity consumption, with **XGBoost** providing the best performance for predicting energy use in Dallas, Texas. Further work can focus on improving the model with additional data, especially real-world consumer reports, and exploring more advanced model architectures.

## Future Work

We plan to:
1. Investigate the use of self-reported consumer data to enhance model accuracy.
2. Further refine models to provide actionable, user-friendly insights for consumers.
3. Explore the deployment of this system for real-time predictions.


For further inquiries, please contact the authors at:
- **Aitor Elfau**: aelfaugonzalez@smu.edu
- **Abdul Wasay**: awasay@smu.edu

