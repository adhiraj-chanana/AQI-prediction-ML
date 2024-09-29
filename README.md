# Air Quality Data Analysis

## Overview

This project analyzes air quality data, focusing on PM10 and other pollutants, using a dataset from Delhi. The analysis includes two main components: a time series analysis of PM10 levels and a regression analysis to predict PM10 based on various features.

## Time Series Analysis

### Description

The time series analysis aims to investigate trends and stationarity in PM10 levels over time. It employs rolling mean and standard deviation calculations, as well as stationarity tests.

### Key Steps

1. **Data Upload and Cleaning**:
   - Load the dataset using Google Colab.
   - Convert the time column to datetime format and handle missing values.
   - Replace zeros in pollutant columns with the mean of those columns.

2. **Exploratory Data Analysis**:
   - Visualize PM10 levels over time.
   - Calculate rolling statistics (mean and standard deviation).

3. **Stationarity Tests**:
   - Perform the Augmented Dickey-Fuller test to assess stationarity.

4. **Modeling**:
   - Use ARIMA to model PM10 levels.
   - Train and evaluate the model using RMSE.

### Code

Refer to the Jupyter Notebook `regression.ipynb` for the complete implementation of the time series analysis.

## Regression Analysis

### Description

The regression analysis predicts PM10 levels using various features from the dataset, such as date and time encoding, using multiple regression techniques.

### Key Steps

1. **Data Upload and Preprocessing**:
   - Load the dataset and examine its structure.
   - Encode categorical variables such as days and times.

2. **Feature Engineering**:
   - Create new features from the existing columns.
   - Drop unnecessary columns to prepare the feature set.

3. **Modeling**:
   - Implement Linear Regression, Random Forest, and Support Vector Regression (SVR).
   - Evaluate each model's performance using RMSE and R² scores.

4. **One-Hot Encoding**:
   - Use one-hot encoding for categorical features and re-evaluate model performance.

5. **Weekend vs. Weekday Analysis**:
   - Analyze the effect of weekends on PM10 levels and assess model performance.

### Code

Refer to the Jupyter Notebook `regression.ipynb` for the complete implementation of the regression analysis.

## Conclusion

This project provides insights into air quality levels in Delhi through time series analysis and regression modeling. The findings can inform policy and decision-making to improve air quality.

## License

This project is licensed under the MIT License.
