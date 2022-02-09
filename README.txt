# Project Name
> Outline a brief description of your project.
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. 

The company wants to know:

1.Which variables are significant in predicting the price of a house, and

2. How well those variables describe the price of a house.

## Table of Contents
* This housing company problem statement. Need to find the predication of house  price for Surprise Housing company.

* python 3 and Git as CM(#technologies-used)




## General Information
Assignment - Advanced Regression

A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. The data is provided in the CSV file below.

The company is looking at prospective properties to buy to enter the market. You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties and decide whether to invest in them or not.

The company wants to know:

Which variables are significant in predicting the price of a house, and

How well those variables describe the price of a house.

Business Goal

You are required to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the


Reading and Understanding the Data

Preparing data set for modeling, rescaleing(Traing vs Test data set)

Training the model

Residual Analysis

Predition and evalution on Test data set

Apply Lasso and Rigde and perform analysis

train.csv is used

* Conclusion:
optimum value Alpha for Lasso is 0.0001 and Alpha for ridge is 4.0

Top 5 features  Rigde and Lassoodel

Ridge	Lasso
GrLivArea	
1stFlrSF	
TotalBsmtSF	
OverallQual_10	
BsmtFinSF1	

Lasso

GrLivArea
OverallQual_10
TotalBsmtSF
OverallQual_9
LotArea

Lasso model is better because it makes features selection and makes 212 coff as 0.it removes those features which does not make much impact in prediction.

Linear model is bad model improved after applying Ridge and Lasso. But Lass model is best.



## Technologies Used
python 3 and Git as CM(#technologies-used)

import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn import linear_model, metrics
from sklearn.linear_model import LinearRegression
from sklearn.linear_model import Ridge
from sklearn.linear_model import Lasso
from sklearn.model_selection import GridSearchCV
from sklearn.metrics import mean_squared_error, r2_score
from sklearn.preprocessing import MinMaxScaler
from sklearn.model_selection import train_test_split
import os


## Acknowledgements
Give credit here.
Thanks to Yash class instructor for explaining the project


## Contact
Created by sandipan.kr@gmail.com


