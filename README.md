# Data Science Lead Scoring Case Study: Project Overview
---
* Created a logistic regression model that helps in identifying potential lead to organisation 
* 

## Code and Resources Used
---
**Python Version:** 3.7
**Packages:** Pandas, numpy, sklearn, matplotlib, seaborn, statsmodel

## Data Cleaning:
---
* Replacing `select` in data with `NaN` as these were the category were customer selected nothing which means a NaN object
* Dropping records which has no use for analysis
* Calculated percentage of **misiisng values** and treated with mean imputation for certain columns
* Inspected numerical columns for **outliers** and capped to 99 percentile

## EDA
---
I looked at the distribution of data and tried to identify the most important feature in the columns that well explains the leads as well as conversion of customers
* performed Univariate and bivariate Analysis 
* found the maximum correlation object with respect to target variable

