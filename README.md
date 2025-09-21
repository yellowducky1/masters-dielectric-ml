# Predicting Refractive Index with Machine Learning

This project explores machine learning techniques for predicting the refractive index of materials using the **Matbench Dielectric dataset**, completed as part of a master's module at Imperial College London.

## Dataset
- Source: [Matbench Dielectric](https://matbench.materialsproject.org/)
- Target: Refractive index of materials

## Preprocessing & Feature Engineering
- Log and Quantile transformations to normalise target distribution
- Feature extraction using **Matminer**
- Feature selection via:
  - Mutual Information
  - Recursive Feature Elimination (RFE)
  - SHAP values for interpretability

## Models Tested
- Ridge Regression
- Decision Trees
- Random Forest
- XGBoost
- CatBoost
- Neural Networks

### Evaluation Metrics
- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)
- Maximum Error
- R² Score

## Optimisation
- Hyperparameter tuning with **Optuna**
- Best model: **XGBoost**, achieving:
  - MAE: 0.3808  
  - RMSE: 1.0687  
  - Max Error: 16.1511  
  - R² Score: 0.6058

## Visuals
- Histograms of transformations
- SHAP feature importance plots
- Predicted vs actual scatter plot

## Skills Demonstrated
- Data cleaning and transformation
- Feature engineering and selection
- Model evaluation and cross-validation
- Hyperparameter tuning
- Visualisation and interpretation

## Future Work
- Address remaining outliers and high max error
- Explore deeper architectures and ensemble methods
- Refine feature engineering for improved R² performance
