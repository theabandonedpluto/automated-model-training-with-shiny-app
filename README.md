# Automated Model Training with ShinyApp
## Overview
This project was developed as part of the advanced R course in a master's degree program. The goal of the project was to create a user-friendly Shiny application that automates the process of generating model metrics for decision tree models, with a focus on random forest.

## Features
The Shiny application consists of three main menus:

### 1. Data Cleaning
In the data cleaning menu, users can upload their dataset in CSV format and preview its contents. The following data cleaning options are available:
NA Value Handling: Users can choose to omit the rows with NA values or replace the NA values with the mean or median of the respective columns.
Value Conversion: Users can convert the values of each column/variable to factors, integers, numerical values, and other appropriate data types.

### 2. Data Visualization
In this menu, users can visualize their data before modeling. The following feature plots are provided:
Frequency Plot: Shows the distribution of values for each variable in the dataset.
Variable Plots: Provides visual representations of each variable, allowing users to gain insights into their data.

### 3. Model
After completing data cleaning and visualization, users can proceed to the model menu, which includes the following functionalities:
Data Preparation: Users can select the target variable, independent variables, and the proportion for splitting the dataset into training and test sets.
Model Selection: Users can specify the parameters required for the random forest model and choose whether to perform regression or classification.
Metrics: Users can view the model metrics, such as accuracy and confusion matrix for classification models, and metrics like MAPE (Mean Absolute Percentage Error) and MAE (Mean Absolute Error) for regression models. Plots related to the chosen model are also displayed.
