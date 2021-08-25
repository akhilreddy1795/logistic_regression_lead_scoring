# Data Science Lead Scoring Case Study: Project Overview
---
* Created a logistic regression model that helps in identifying potential lead conversion rate to organisation 
* Optimized model to provide **92% on test accuracy**

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
![lead score github](https://user-images.githubusercontent.com/69252134/130774568-e5be5ba2-c48c-4cd8-9ffc-985fd7bc8b5e.png)

## Model Building
---
First, I transformed the categorical variables into **dummy variables**. I also split the data into **train and test** sets with a test size of 30%.

* I started building the model using **Stats model and RFE**
* PLotted **ROC curve and got area of 0.97**
* PLotted `Accuracy, sensitivity and specificity` for various probabilities to find the cut off
![cut off lead score git hub](https://user-images.githubusercontent.com/69252134/130775695-1460e8a9-9d70-4f0f-a759-ffff21149492.png)
<br>Here we selected **0.3** as probability cut off

## Model Performance 
---
we got final Test accuracies as

* **Accuracy:** 92.21%
* **Sensitivity:** 91.78%
* **Specificity:** 92.48%

MOdel seems to predict the target lead conversion Rate very well
