# Rossmann-Store-Sales-Prediction
Transform sales forecasting for Rossmann store with our high-accuracy XGBoost model. Leverage advanced data analysis, feature engineering, and machine learning techniques to predict sales up to six weeks in advance.

This repository contains the code and documentation for the Rossman Sales Prediction project. The goal of this project is to forecast the daily sales of Rossmann stores for up to six weeks in advance. By accurately predicting sales, store managers can make informed decisions regarding promotions, competition, holidays, and other factors that influence sales performance.

## Problem Statement
Rossmann operates over 3,000 drug stores across 7 European countries. Currently, store managers rely on their own predictions for daily sales, leading to varying levels of accuracy. The objective of this project is to develop a machine learning model that can forecast the "Sales" column for the test set. The [dataset](https://www.kaggle.com/c/rossmann-store-sales/data) provided includes historical sales data for 1,115 Rossmann stores, taking into account factors such as promotions, competition, school and state holidays, seasonality, and store locality. It is worth noting that some stores in the dataset were temporarily closed for refurbishment.

## Project Summary

The Rossman Sales Prediction project involved extensive data analysis, feature engineering, and model selection to accurately forecast sales. Here is a brief overview of the project steps and key findings:

**1. Data Gathering and Cleaning:**

 * Collected historical sales data for Rossmann stores, including competitor details, holidays, customer count, and daily sales.
 * Performed data cleaning to handle missing values and ensure data consistency.
 * Merged relevant datasets to enhance the feature set.

**2. Exploratory Data Analysis (EDA) and Visualization:**

* Study the distributions of individual columns (uniform, normal, exponential).
* Detect anomalies or errors in the data (e.g. missing/incorrect values).
* Study the relationship of target column with other columns (linear, non-linear etc.)
* Generated insightful visualizations to uncover patterns and trends in the data.
* Came up with ideas for preprocessing and feature engineering.

**3. Feature Engineering and Preprocessing:**

* Created additional features such as Promo2Open and CompetitionOpen to capture relevant information.
* Imputed Missing numeric data using SimpleImputer as machine learning model can't work with missing numerical data.
* Scaled Numeric Features using MinMaxScaler
* Encoded categorical variables using One-Hot Encoding for compatibility with machine learning algorithms.

**4. Model Selection and Training:**

* Split the preprocessed data into training and validation sets.
* Utilized a variety of machine learning algorithms, including linear regression, decision trees, random forests, and XGBoost.
* Evaluated model performance using metrics such as Root Mean Squared Error(RMSE).
* Employed regularization techniques (e.g., Lasso, Ridge, Elastic Net) for improved model performance.
* Identified XGBoost as the optimal model due to its high accuracy and with less RMSE compared to all other model. we got accuracy_score of 0.98 on training as well as validation dataset

**5. Model Deployment and Conclusion:**

* Finalized the XGBoost model for deployment, as it demonstrated the highest accuracy and the least error.
* Developed a comprehensive machine learning pipeline that combines data processing, feature engineering, and model evaluation, saved a model in a pickle file which we can use for deployment.
* Successfully created a model capable of accurately predicting sales for Rossmann stores up to six weeks in advance.

This project showcases the effective utilization of data analysis, feature engineering, and machine learning techniques to solve a real-world forecasting problem. The insights gained from the analysis provide valuable information for decision-making within the retail industry.
