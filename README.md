# Global Inflation Analysis with Machine Learning

This project explores global inflation rates across countries and applies a simple machine learning model to forecast the next year’s inflation.

## Project Overview

### 1.Data Loading & Cleaning
    1. Import the global inflation dataset (global_inflation_data.csv).
    2. Drop irrelevant columns (e.g., indicator_name).
    3. Handle missing values using mean imputation.

### 2.Data Preprocessing
    1. Scale numerical values with StandardScaler.
    2. Reshape the dataset into a long format: country, year, inflation_rate.
    3. Create lag features (t-1, t-2) for time-series style prediction.

### 3.Modeling
    1. Train a Linear Regression model using lag features.
    2. Predict inflation for the next year based on the last two years.
    3. Evaluate model performance with RMSE.

### 4.Forecasting
    1. Choose a country (e.g., United States).
    2. Predict its next year’s inflation using the trained model.
    3. Display both:
        1. Scaled value (z-score, mean=0, std=1).
        2. Real value (converted back to % inflation).

### 5. Visualization
    1. Plot historical inflation data for a country.
    2. Add a red dot for the predicted next year’s inflation.

## Example Output
    
    1. Prediction for United States in 2025:
    2. Scaled value: 0.18
    3. Real value: 3.42%
    4. The plot shows the historical trend in scaled values, with a red dot marking the predicted inflation.
## Run in Google Colab  
    You can open this notebook directly in Google Colab using the link below: 
    https://colab.research.google.com/drive/11pkBp6pIHYF_2OqeDjffZ_YN56RywNkF?usp=sharing
