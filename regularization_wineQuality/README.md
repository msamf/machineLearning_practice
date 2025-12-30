# Regularization: Wine Quality

## Introduction
This project explores regularization (ridge and lasso) based on a logistic regression model to predict wine quality. 
Note: Project is based on Codecademy's [Regulatrization](https://www.codecademy.com/paths/fe-path-feature-engineering/tracks/fe-feature-selection-methods/modules/fe-regularization/projects/fe-logistic-regression-with-regularization) project. 

## Dataset
The dataset is red wine quality from UCI's [Wine Quality](https://archive.ics.uci.edu/dataset/186/wine+quality). Provided information includes fixed acidity, volatile acidity, citric acid, residual sugar, chlorides, and more. 

## Methods
The following steps are performed (after library imports and data loading):
1. Target variable "quality" is mapped to binary 0/1 to enable logistic regression
1. Data is scaled via StandardScaler()
1. Logistic regression (LR) model with no regularization is trained and evaluated
1. LR model with L2 regularization is trained and evaluated
    * Hyperparameter C is then tuned to find best model with L2 regularization
1. LR model with L1 regularization is trained (including hyperparameter C tuning)

## Results and Conclusion
Method | Train Score | Test Score
-- | -- | --
No Reg | 0.773 | 0.727
L2 Reg (best C=0.0021) | 0.770 | 0.735
L3 Reg (best C=1.5) | 0.773 | 0.727

L2 Reg had similar training scores as No Reg, but performed better in the test set. L3 Reg performed at the same level as No Reg, but had one of the coefficient as 0 so effectively removed a feature. 