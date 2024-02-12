# Forecasting Serious Delinquency Rate in R Markdown
## Executive Summary
The serious delinquency rate, defined as loans 90 days or more past due including those in foreclosure, poses significant risks to banks' financial stability. Without accurate forecasting, banks may face increased risk exposure and revenue losses. This report explores various models to forecast the serious delinquency rate, with Median Quantile Regression emerging as the most accurate model, achieving an 87.07% accuracy rate when forecasting four quarters ahead.

## Section 1: Overview
Delinquency occurs when borrowers fail to make loan payments on time, putting loans at risk of default. The serious delinquency rate, categorized as loans 90 days or more past due, including those in foreclosure, is a crucial metric for assessing financial risk. This report utilizes both Parametric and Non-Parametric Models to forecast delinquency rates. Parametric models, with fixed parameters, offer computational speed but rely on strong assumptions about data. Non-parametric models, with flexible parameters, make fewer assumptions but require more data. Exploratory data analysis is conducted to understand the data structure, followed by model construction to identify significant variables. With recent economic changes, the model assesses if the unemployment rate is a reliable predictor of mortgage delinquency rates.

## Section 2: Exploratory Data Analysis
This section involves reading and visualizing data, as well as testing for variable correlations to ensure data suitability for parametric and non-parametric models.

![image](https://github.com/jvick1/R_Studio_DQ_Forecasting/assets/32043066/bc25ee6a-14c6-4e39-876e-aa2842c9c6e6)

![image](https://github.com/jvick1/R_Studio_DQ_Forecasting/assets/32043066/bb7f6cd4-34a6-4bff-a531-cd54c9a82e08)

## Section 3: Parametric Model
Parametric machine learning algorithms, such as linear regression, offer ease of interpretation and speed but are limited in complexity. The report tests linear regression with all variables and statistically significant variables, along with logistic regression classification (LRC), linear discriminant analysis (LDA), and quadratic discriminant analysis (QDA).

![image](https://github.com/jvick1/R_Studio_DQ_Forecasting/assets/32043066/5a234917-62ce-41b4-a320-a91e7f293475)

## Section 4: Non-Parametric Model
Non-parametric methods, aiming to find the best fit for training data while generalizing to unseen data, offer flexibility but require more data and risk overfitting. Models tested include decision trees, quantile regression, local regression, and k-nearest neighbor (K-NN) classification. Mean Squared Error (MSE) comparison reveals that Quantile Regression has the lowest MSE among non-parametric models, while Linear Model (Sig) has the lowest MSE overall among parametric models tested.

![image](https://github.com/jvick1/R_Studio_DQ_Forecasting/assets/32043066/d5684b12-1370-44a3-99db-7e91d8ec9fef)

This comprehensive analysis underscores the importance of selecting appropriate models for forecasting serious delinquency rates, with Median Quantile Regression emerging as the most accurate choice for the task.
