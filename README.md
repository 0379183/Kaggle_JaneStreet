# Kaggle_JaneStreet (Financial Time-Series Prediction)

This competition focused on predicting future stock returns using real-world trading data, framed as a regression problem evaluated via R-squared (R²). Our goal was to model market behavior across short- and medium-term time horizons.

## Instructions
1）Download the competition data in the following：
https://www.kaggle.com/competitions/jane-street-real-time-market-data-forecasting/data

2）Run nn_train.ipynb,ridge_train.ipynb,xgb_train.ipynb,tabm_train.ipynb files for getting model weight

3）Run ensemble.ipynb file

Note: This project requires at least one GPU and a minimum of 64 GB of RAM.

## Summary

**Featured engineering**
- Constructed composite indicators by calculating differences and products between 79 anonymized features, forming a market index correlation matrix to capture latent interactions.
- Applied time-series sliding windows (1/2/3/5/10) to extract statistical patterns (mean, variance, etc.), effectively capturing trend and periodicity.

**Model Selection**
- Used LightGBM, CatBoost, XGBoost, and deep MLPs tailored to the data structure.
- Employed TimeSeriesSplit to partition by trading day, preventing overfitting and ensuring generalization.
- Tuned models via grid search and Bayesian optimization.

**Results**
- Our solution ranked in the top 3% among 3,000+ global teams.
- Demonstrated advanced feature design, robust modeling, and disciplined project pacing.

This experience deepened our understanding of structured modeling for financial time-series, with implications for future adversarial and security forecasting research.
