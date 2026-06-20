# House Price Prediction

## Project Overview

This project aims to predict house prices using machine learning techniques based on various property characteristics such as area, number of bedrooms, bathrooms, parking availability, furnishing status, and location-related features. The goal is to build predictive models, evaluate their performance, and identify the factors that have the greatest impact on house prices.

## Dataset

* Dataset Name: Housing Prices Dataset
* Source: Kaggle
* Records: 545
* Features: 13
* Target Variable: `price`

The dataset contains information about residential properties, including both numerical and categorical features.

### Features Used

* area
* bedrooms
* bathrooms
* stories
* mainroad
* guestroom
* basement
* hotwaterheating
* airconditioning
* parking
* prefarea
* furnishingstatus

## Project Workflow

### 1. Data Loading and Exploration

* Loaded the dataset using Pandas.
* Examined dataset structure and feature information.
* Checked for missing values and duplicates.

### 2. Data Cleaning and Preprocessing

* Removed duplicate records if present.
* Verified that there were no missing values.
* Converted categorical variables into numerical format using One-Hot Encoding.
* Prepared the dataset for machine learning models.

### 3. Model Building

Two regression models were trained and evaluated:

#### Linear Regression

A baseline regression model used to predict house prices.

#### Random Forest Regressor

An ensemble learning model used to capture more complex relationships in the data.

The dataset was split into training and testing sets using an 80:20 ratio.

## Model Performance

Linear Regression

* MAE = 970,043
* RMSE = 1,324,507
* R² Score = 0.653

Random Forest Regressor

* MAE = 1,006,663
* RMSE = 1,383,659
* R² Score = 0.621

### Best Model

Linear Regression achieved better performance with lower prediction errors and a higher R² score.

## Visualizations

The following visualizations were created:

1. House Price Distribution Histogram
2. Correlation Heatmap
3. Actual vs Predicted Price Scatter Plot

These charts helped analyze data distribution, feature relationships, and model performance.

## Key Findings

* Area is the most influential factor affecting house prices.
* Bathrooms, bedrooms, parking availability, and air conditioning significantly impact property value.
* Preferred residential areas tend to have higher house prices.
* The Linear Regression model explained approximately 65% of the variation in house prices.

## Business Recommendation

Real estate companies should focus on larger properties located in preferred residential areas and emphasize amenities such as air conditioning, parking facilities, and multiple bathrooms during marketing campaigns. These features contribute significantly to higher property values and improved sales potential.

## Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

## Project Structure

HousePricePrediction_[YourName]/

├── analysis.ipynb

├── Housing.csv

├── summary.pdf

├── README.md

└── charts/

    ├── price_distribution.png

    ├── correlation_heatmap.png

    └── actual_vs_predicted.png
