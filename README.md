# Predictive Modeling for Car Prices

## Introduction
This document outlines the process of building a predictive model to estimate car prices using machine learning techniques. The dataset used for this analysis contains information about various attributes of cars, such as mileage, transmission type, fuel type, and engine size.

## Data Exploration
Importing necessary libraries: pandas, matplotlib.pyplot, seaborn, and sklearn.
Loading the dataset from the CSV file ford.csv using pd.read_csv() function.
Displaying the first few rows of the dataset using car_dataset.head() to understand its structure.
Checking the shape of the dataset to determine the number of rows and columns.
Using car_dataset.info() to get information about the dataset, including data types and missing values.
Describing the statistical summary of the dataset using car_dataset.describe().
Checking for missing values in the dataset using car_dataset.isnull().sum().
Printing the counts of unique values for the 'transmission' and 'fuelType' columns.

## Data Preprocessing
Replacing categorical values in the 'transmission' column with numerical values: 'Manual' with 0, 'Automatic' with 1, and 'Semi-Auto' with 2.
Replacing categorical values in the 'fuelType' column with numerical values: 'Petrol' with 0, 'Diesel' with 1, 'Hybrid' with 2, 'Electric' with 3, and 'Other' with 4.
Splitting the dataset into features (X) and target variable (Y), dropping the 'model' and 'price' columns from features.
Splitting the dataset into training and testing sets using train_test_split() from sklearn.model_selection.

## Model Training
Initializing a Linear Regression model and fitting it to the training data using LinearRegression().
Making predictions on the training data and calculating the R-squared error.
Plotting the scatter plot between actual and predicted prices for training data.

## Model Evaluation
Making predictions on the testing data using the trained Linear Regression model.
Calculating the R-squared error for the testing data.
Plotting the scatter plot between actual and predicted prices for testing data.
