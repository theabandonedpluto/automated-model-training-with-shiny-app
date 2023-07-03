# Automated Model Training with ShinyApp
## Overview
This project was developed as part of the advanced R course in a master's degree program. The goal of the project was to create a user-friendly Shiny application that automates the process of generating model metrics for decision tree models, with a focus on random forest.

## Features
The Shiny application consists of three main menus:

### 1. Data Cleaning
In the data cleaning menu, users can upload their dataset in CSV format and preview its contents. The following data cleaning options are available:
* Upload Data : Users can upload their csv dataset and see the summary of the data
* NA Value Handling: Users can choose to omit the rows with NA values or replace the NA values with the mean or median of the respective columns.
* Value Conversion: Users can convert the values of each column/variable to factors, integers, numerical values, and other appropriate data types.

### 2. Data Visualization
In this menu, users can visualize their data before modeling. The following feature plots are provided:
* Frequency Plot: Shows the distribution of values for each variable in the dataset.
* Variable Plots: Provides visual representations of each variable, allowing users to gain insights into their data.

### 3. Model
After completing data cleaning and visualization, users can proceed to the model menu, which includes the following functionalities:
* Data Preparation: Users can select the target variable, independent variables, and the proportion for splitting the dataset into training and test sets.
* Model Selection: Users can specify the parameters required for the random forest model and choose whether to perform regression or classification.
* Metrics: Users can view the model metrics, such as accuracy and confusion matrix for classification models, and metrics such as: MAPE (Mean Absolute Percentage Error) and MAE (Mean Absolute Error) for regression models. Plots related to the chosen model are also displayed.

## Files Documentation
### Shiny Apps:
1. templateShinyFinal.R <- the shiny application (UI & Server): defensive programming, shiny 
app
2. trainers_classes.R <- machine learning model (classes & objects) : R6 OOP
3. medical.csv <- csv file to test in the shiny app

### Package ML:
1. Folder:MyFirstPacakge <- the developer's codes for the package
2. autoforest.tar.gz <- the package including vectorization created from trainers_classes.R
3. DfFunction.cpp <- c++ functions to show basic information of dataframe
4. medical_train_test.RData <- the same with medical.csv
5. package_demo.R <- R script to test autoforest package and c++ functions with medical Rdata
