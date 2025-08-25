# Global Inflation Analysis with Machine Learning

This project explores global inflation rates across countries and applies a simple machine learning model to forecast the next year’s inflation.

## Project Overview

### 1.Data Loading & Cleaning
    Import the global inflation dataset (global_inflation_data.csv).
    Drop irrelevant columns (e.g., indicator_name).
    Handle missing values using mean imputation.

### 2.Data Preprocessing
    Scale numerical values with StandardScaler.
    Reshape the dataset into a long format: country, year, inflation_rate.
    Create lag features (t-1, t-2) for time-series style prediction.

### 3.Modeling
    Train a Linear Regression model using lag features.
    Predict inflation for the next year based on the last two years.
    Evaluate model performance with RMSE.

### 4.Forecasting
    Choose a country (e.g., United States).
    Predict its next year’s inflation using the trained model.
    Display both:
        Scaled value (z-score, mean=0, std=1).
        Real value (converted back to % inflation).

### 5. Visualization
    Plot historical inflation data for a country.
    Add a red dot for the predicted next year’s inflation.

## Example Output

    Prediction for United States in 2025:
    Scaled value: 0.18
    Real value: 3.42%
    The plot shows the historical trend in scaled values, with a red dot marking the predicted inflation.