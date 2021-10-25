# Rainfall_Prediction

## Project Overview
Obtained the dataset using Kaggle and implemented three rainfall prediction models, namely; Support Vector Regression, Random Forest regressor and Decision Tree Regressor.
Performed the pre-processing, feature engineering, EDA and implemented machine learning models using R Script.
Hypertuned the models for better accuracy.
All the three models with the least RMSE among all the experiments are as follows:
Decision Tree Regressor (70:30 split): 0.2859088
Random Forest Regressor (ntree=500): 0.1569539
Support Vector Regressor (Feature scaled data): 0.02646819

## Introduction and Motivation behind the Project
* Many researchers have focused on rainfall forecasting over the years. Rainfall prediction is one of the most critical aspects of economic growth in a country like India, where agriculture is one of the most important sectors. According to a study (Shah et al., 2018), precipitation forecasting is one of the most important investigations in meteorological science. Because of the existence of non-linearity and instabilities in the environment, it is difficult to forecast the Indian monsoon, which leads to the use of various machine learning models to solve the problem (Dash et al., 2018). Hence, this project focuses on identifying the most important factor responsible for rainfall and using the best machine learning model with highest accuracy for rainfall prediction.

## Result
* This study provided a good opportunity to develop comprehensive machine learning model for a real-world problem i.e., the rainfall prediction. Since heavy rainfalls or no rainfalls can cause several issues, it is important to develop machine learning models with high performance that are used not only to classify rainfall but all able to predict the rainfall for upcoming days or months using regression models. 
* In this study, several machine learning models were studied among which the decision tree regression, random forest regression and support vector regression were used. These models were implemented on the Austin-weather dataset and along with tuning, feature scaling and feature selections, the support vector regression performed the best based on the RMSE score. The RMSE score was used to evaluate the performance of the models. 
