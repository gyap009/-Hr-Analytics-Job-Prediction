# HR-Analytics-Job-Prediction

**Google Advanced Data Analytics Course: Capstone Project**

## Overview
This project aims to predict employee attrition in a company using a machine learning model. By identifying the factors that contribute to employees leaving the company, we can make informed recommendations to improve employee satisfaction and retention.

## Problem Statement
The HR department wants to take initiatives to improve employee satisfaction levels at the company. By predicting employees likely to quit, it might be possible to identify factors that contribute to their departure. This is crucial because finding, interviewing, and hiring new employees is time-consuming and expensive. Increasing employee retention will be beneficial to the company.

## Goal
Analyze the data collected by the HR department and build a regression/machine learning model that predicts whether an employee will leave the company.

## Dataset
The dataset used in this project is provided by the HR department and contains the following columns:

- `satisfaction_level`
- `last_evaluation`
- `number_project`
- `average_monthly_hours`
- `tenure` (renamed from `time_spend_company`)
- `work_accident`
- `left` (target variable)
- `promotion_last_5years`
- `department`
- `salary`

## Data Exploration and Cleaning
Initial data exploration and cleaning steps included:

1. Loading the dataset
2. Standardizing column names to snake_case
3. Checking for missing values and duplicates
4. Removing duplicates
5. Handling outliers in `tenure`

## Data Visualization
Data visualization was conducted to gain insights into the dataset:

- Boxplot to detect outliers for tenure
- Monthly hours by number of projects
- Scatterplot of average monthly hours vs. satisfaction level
- Histogram of counts of stayed/left by department
- Correlation heatmap

## Data Modeling
A logistic regression model was used to predict employee attrition:

1. Encoding non-numeric variables
2. Feature selection
3. Splitting data into training and testing sets
4. Training the logistic regression model
5. Making predictions and evaluating the model

## Model Evaluation
The model was evaluated using various metrics:

- Confusion Matrix
- Classification Report

## Insights and Recommendations
Based on the analysis and model results, the following recommendations were made to improve employee retention:

1. Cap the number of projects that employees can work on.
2. Consider promoting employees who have been with the company for at least four years or investigate why these employees are dissatisfied.
3. Reward employees for working longer hours or avoid requiring them to do so.
4. Inform employees about overtime pay policies and clarify workload and time-off expectations.
5. Hold company-wide and team-specific discussions to address work culture issues.
6. Use a proportionate scale for rewarding employees who contribute more or put in more effort.

## Conclusion
The logistic regression model achieved an accuracy of 83% and provided valuable insights into factors contributing to employee attrition. By implementing the recommendations, the company can improve employee satisfaction and retention, thereby reducing the costs and efforts associated with hiring new employees.
