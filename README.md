# Sleep Disorder Study

This is a final project for ADS503: Applied Predictive Modeling [https://github.com/VSbr22/ADS503-Group-Project](https://github.com/VSbr22/ADS503-Group-Project)

#### -- Project Status: [Completed]

## Project Intro
The purpose of this project is to present the process used to determine the best set of features to predict a patients likelihood of having a sleep disorder. Binary classification models employed for this research project include Logisitic Regression, Bagging, XgBoost, Random Forests, NeuralNet, Penalized GLM, Linear Discriminant Analysis, and Nearest Shrunken Centroids. 5-fold cross validation was deployed to evaluate and find the best tuning parameters to optimize our models. Based on the results of the classification models it has been determined that the models are effective and determing the presence or absence of a sleep disorder. 


### Team 3
* Joel Day
* Diana Arbas
* Vannesa Salazar


### Methods Used
* Data preprocessing
* Exploratory Data Analysis
* Data Visualization
* Predictive Modeling


### Technologies
* R
* RStudio, jupyternotebook


## Project Description
-Predicting the presence or absence of a sleep disorder can be life changing for a patient. Based on the severity of the disorder it is important to correctly classify a disorder when it is present and not when it is absent. Determining a diagnosis is very high stakes and can be detremental to a patients health with a correct diagnosis or misdiagnosis. 
- Developing a standard of care with classification in mind and seeing what impacts the presence of a sleep disorder.  
- By predicting the presence of a sleep disorder a patient can be made aware and take actionable steps to better their sleep health. 
- The results of a medical misdiagnosis could potentially lead to medical malpractice. 
- Medical misdiagnosis cause a patient a negative medical outcome, over or undertreatment, delayed recovery, stress, anxiety, umongst other negative outsomes.
- Dataset provided by Kaggle 
- Sleep Dataset: https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset



## Needs of this project

- data exploration/descriptive statistics
- data processing/cleaning
- statistical modeling
- writeup/reporting
- presentation
- voice recordings

## Required Python Packages
* library(ggplot2)
* library(gridExtra)
* library(caret)
* library(tidyverse)
* library(corrplot)
* library(dplyr)
* library(ggfortify)
* library(pROC)
* library(MLmetrics)
* library(glmnet)
* library(gbm)
* library(randomForest)
* library(adabag)
* library(xgboost)

## Getting Started

1. Clone this repo using raw data.
2. add code and push new code into repo. To ensure cohesive code make sure to run all cells prior to upload. 

## Featured Notebooks/Analysis/Deliverables
* [Presentation slides ]
* https://github.com/VSbr22/ADS503-Group-Project/blob/09b218f51ba5a83a9a43b9c240969bb376c533bc/Techincal%20Presentation.pptx
* 


## Data Pre-Processing
* The class imbalance of the response variable was corrected using stratified sampling. The response variable was also changed to a binary variable of either having a sleep disorder (1) or not (0). 
* Irrelevant and redundant predictors were dropped from the dataset specifically the duplicate column of Sleep Disorder, and Person ID.
Test/Training set was created with a more balanced response variable being depicted in both sets. 
* Blood pressure column was split into two columns one for Systolic, and Diastolic numbers corresponding to the readings of a blood pressure screening. They were then transformed to numeric values.
* Blood Pressures were binned using thresholds for low, normal, high blood pressure. Original columns removed after. 
* Dummy variables were created for the categorical predictors Occupation and BMI Category.  Resulting in more attributes for the dataset to encompass a variety of employments and BMI types. 
* Near-zero variance predictors were removed for feature reduction. 
* Check for multicollinearity using a correlation matrix.  Depending on the model some features will be removed due to high correlation, and some will be kept. 
* Gender is transformed from Male/Female to 0/1. 
* Center & Scaling of predictor variables to get the distribution to normal like.
* Replace response variable in BMI category to combine two duplicate response. (Normal Weight and Normal combined)


## Exploratory Data Analysis
* Verified dimenstion and summary of the dataset
* verified no missing values
* verified there is an imbalance in the response variable
* Verified a duplicate response type in BMI category
* Various data types, numerical, ordinal, categorical.




## Features Selection
* Correlation to Target 
* Near Zero Variance Variables removed


## Modeling & Evaluation
* Logistic Regression
* Nearest Shrunken Centroid
* AdaBoost
* Random Forest
* XGboost
* Penalized GLM
* Boosting
* Neural Net
