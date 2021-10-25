# Rainfall_Prediction

## Project Overview
* Obtained the dataset using Kaggle and implemented three rainfall prediction models, namely; Support Vector Regression, Random Forest regressor and Decision Tree Regressor.
* Performed the pre-processing, feature engineering, Exploratory Data Analysis and implemention of machine learning models all using R Script.
* Hypertuned the models for better accuracy.
* All the three models with the least RMSE among all the experiments are as follows:
* Decision Tree Regressor (70:30 split): 0.2859088
* Random Forest Regressor (ntree=500): 0.1569539
* Support Vector Regressor (Feature scaled data): 0.02646819

## Code and Resources Used

R Studio
Libraries: dplyr, DataExplorer, reshape2, ggplot2, Boruta, mlbench, caret, randomForest, e1071, caTools, rpart, rpart.plot
[Dataset]: (https://www.kaggle.com/grubenm/austin-weather)


## EDA
![image](https://user-images.githubusercontent.com/72705368/138744782-5ae43af5-85a9-4322-857c-5880e9f4aaf7.png)

### Historgram plot for Numerical Variables
![image](https://user-images.githubusercontent.com/72705368/138744869-341172b8-174e-4825-afaf-16fee9956e1c.png)

### Correlation Matrix for Feature Selection
![image](https://user-images.githubusercontent.com/72705368/138745118-2ce49573-e277-4ff5-bed9-5550552afd80.png)

### Importance Plot for features using the Boruta Package
* By using Boruta package for feature selection and on the basis correlation heatmap, it can be concluded that variables TempHighF, TempAvgF, TempLowF, DewPointHighF, DewPointAvgF, DewPointLowF, HumidityAvgPercent, HumidityLowPercent, VisibilityAvgMiles, VisibilityLowMiles, WindHighMPH, WindAvgMPH, WindGustMPH are important and the variable SeaLevelPressureAvgInches is a tentative variable.

![image](https://user-images.githubusercontent.com/72705368/138745237-e8a39567-4fbd-4bee-9325-4818923be1ad.png)

## Model Implementation and Performance
First, I did research and decided the models that I will be implementing for this project. Then, I studied the dataset by performing EDA. I used 0.8:0.2 train-test split as well as 0.7:0.3 train-test split.

I tried various experiments on three different models and evaluated the performance using Root Mean Squared Error (RMSE). 

| No. |	Experiment |	Dataset Used |	Model |
| --- | ---------- |  ------------ | ------ |
| 1.	| Decision Tree(70:30 split) |	Normal Dataset |	Decision Tree |
| 2.	| Decision Tree (80:20 split) |	Normal Dataset |	Decision Tree |
| 3.	| Random Forest (ntree = 500) |	Normal Dataset |	Random Forest Regressor |
| 4.	| Random Forest Tuning |	Normal Dataset | Random Forest Regressor |
| 5.	| Random Forest with min MSE (ntree = 62)	| Normal Dataset |	Random Forest Regressor |
| 6.	| Support Vector Regression using RBF Kernel |	Normal Dataset |	Support Vector Regression |
| 7.	| Support Vector Regression using RBF kernel and Feature Selection |	Feature selected Dataset |	Support Vector Regression |
| 8.	| Support Vector Regression using RBF kernel and Feature Scaling	| Feature scaled Dataset | 	Support Vector Regression |
| 9.	| Support Vector Regression using RBF kernel and Feature selection + scaling |	Feature selected and scaled Dataset |	Support Vector Regression |


All the three models with the least RMSE among all the experiments are as follows:
* Decision Tree Regressor (70:30 split): 0.2859088
* Random Forest Regressor (ntree=500): 0.1569539
* Support Vector Regressor (Feature scaled data): 0.02646819

## Conclusion
* In this study, several machine learning models were studied among which the decision tree regression, random forest regression and support vector regression were used. These models were implemented on the Austin-weather dataset and along with tuning, feature scaling and feature selections, the support vector regression performed the best based on the RMSE score. The RMSE score was used to evaluate the performance of the models.

