# R-Projects_Machine_Learning
Collection of machine learning projects in R, including data preprocessing, modeling, and performance evaluation across classification and regression tasks.

1. Gender Statistics and Hapiness Index (EUR Master Course: Introduction to Data Science)

   This project analyzes the relationship between World Bank Gender Statistics and the World Happiness Index (World Happiness Report) to identify which gender-related factors most influence national happiness levels. After data cleaning and merging multiple datasets, dimensionality reduction was performed using PCA (validated with bootstrap and permutation tests), followed by Principal Component Regression (PCR) and Lasso regression with cross-validation for prediction and variable selection. The models were evaluated using MSE and applied to out-of-sample country predictions.

2. Bank Term Deposit Subscription Prediction (EUR Master Course: Seminar Data Science for Marketing Analytics)

   Used the Portuguese Bank Marketing dataset (phone campaign data from 2008–2010; published by Moro, Cortez & Rita / UCI) [Kaggle] to predict whether a customer subscribes to a term deposit after the last contact and identify the most influential campaign and macroeconomic drivers. The workflow included data cleaning (handling “unknown” values), feature engineering (encoding categorical variables, scaling numeric features), class-imbalance handling via ROSE over/under-sampling, and feature selection with Lasso (cv.glmnet). Models compared were LightGBM, CART (rpart with CV tuning), and Random Forest, evaluated mainly with balanced accuracy, sensitivity, specificity, and Cohen’s kappa, followed by feature importance and tree interpretation for insights.

3. Transportation Mode Prediction using Gradient Boosting
   
   This project predicts whether individuals choose public transport or private car for their daily commute using ensemble machine learning techniques on a dataset of 5,896 observations. The primary model implemented is Gradient Boosting (GBM) with 10-fold cross-validation for hyperparameter tuning, while AdaBoost and XGBoost were also tested for comparison. Model performance was evaluated using a confusion matrix and accuracy (~79%), and feature importance analysis revealed that time-related variables, especially the ratio between public transport and car travel time are the most influential factors in transportation mode decisions.

4. Semantic Word Maps via Multidimensional Scaling

    This project visualizes semantic structure in text by building a word co-occurrence matrix from a cleaned review corpus, converting co-occurrence similarities into distances, and applying Multidimensional Scaling (MDS) using smacof to generate interpretable 2D and 3D word maps. The pipeline includes corpus creation, tokenization, DFM/FCM construction with quanteda, selecting the top-N most frequent terms, transforming similarity→distance (sim2diss), and plotting the resulting coordinates as labeled 2D maps (ggplot2) and an interactive 3D label view (plotly), enabling quick exploration of clusters and related terms in the review vocabulary.

   
