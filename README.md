# R-Projects_Machine_Learning
Collection of machine learning projects in R, including data preprocessing, modeling, and performance evaluation across classification and regression tasks.

1. Gender Statistics and Hapiness Index (EUR Master Course: Introduction to Data Science)

   This project analyzes the relationship between World Bank Gender Statistics and the World Happiness Index (World Happiness Report) to identify which gender-related factors most influence national happiness levels. After data cleaning and merging multiple datasets, dimensionality reduction was performed using PCA (validated with bootstrap and permutation tests), followed by Principal Component Regression (PCR) and Lasso regression with cross-validation for prediction and variable selection. The models were evaluated using MSE and applied to out-of-sample country predictions.

2. Bank Term Deposit Subscription Prediction (EUR Master Course: Seminar Data Science for Marketing Analytics)

   Used the Portuguese Bank Marketing dataset (phone campaign data from 2008–2010; published by Moro, Cortez & Rita / UCI) [Kaggle] to predict whether a customer subscribes to a term deposit after the last contact and identify the most influential campaign and macroeconomic drivers. The workflow included data cleaning (handling “unknown” values), feature engineering (encoding categorical variables, scaling numeric features), class-imbalance handling via ROSE over/under-sampling, and feature selection with Lasso (cv.glmnet). Models compared were LightGBM, CART (rpart with CV tuning), and Random Forest, evaluated mainly with balanced accuracy, sensitivity, specificity, and Cohen’s kappa, followed by feature importance and tree interpretation for insights.
   
