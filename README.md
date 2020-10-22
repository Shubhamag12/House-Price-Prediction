# House-Price-Prediction
[]()

## Overview
This is an ML-based application that predicts the house prices based upon the features provided (such as area, num of bedrooms, etc.)
For testing using sample inputs, click [here](https://github.com/Shubhamag12/House-Price-Prediction/blob/main/Delhi_load.ipynb)

Model Used | Accuracy
------------ | -------------
Linear Regressor | 81.705317 (Cost)
Ordinary Least Squares | 92.9 (R-squared value)

File Description:
- **Delhi_load.ipynb** : Application interface for users.
- **CSV File/ Delhi.csv** : dataset
- **Codes/ Delhi.ipynb** : Main file with all processing stuff
- **Codes/ ols_results_delhi.pickle** : Pickled OLS model after training on dataset

## Problem Statement
Given a set of features, predict the price of any given house in the Delhi region.

## Dataset and libraries used

<details open>
  <summary><b>Dataset Summary</b></summary>
  
  
  1. Reference link for dataset : [click here]()
  2. df.info()
  
  ![Image for datafraame summary](https://github.com/Shubhamag12/House-Price-Prediction/blob/main/Images/Dataframe_infpo.png)
</details>

<details>
  <summary>Libraries Used</summary>
  
  1. [Pandas](https://pandas.pydata.org/)
  2. [Statsmodel](https://www.statsmodels.org/)
  3. [Sklearn](https://scikit-learn.org/)
  4. [Numpy](https://numpy.org/)
  5. [Seaborn](https://seaborn.pydata.org/)
  6. [Matplotlib](https://matplotlib.org/)
  7. [Google.colab](https://colab.research.google.com/)
</details>

## Feature analysis

<details>
  <summary>Outliers</summary>
  
  1. Price
  
  Raw Data
  ![Price_outliers](https://github.com/Shubhamag12/House-Price-Prediction/blob/main/Images/Price_outliers.png)
  Rectified Data
  ![Corrected Price](https://github.com/Shubhamag12/House-Price-Prediction/blob/main/Images/Corrected_Price_outliers.png)
  
  2. Area
  
  Raw Data
  ![Area Outliers](https://github.com/Shubhamag12/House-Price-Prediction/blob/main/Images/Area_outliers.png)
  Rectified Data
  ![Corrected Area](https://github.com/Shubhamag12/House-Price-Prediction/blob/main/Images/Corrected_Area_outliers.png)
  
  3. Price per sq. foot
  
  Raw Data
  ![Price/ Sq. foot Outliers](https://github.com/Shubhamag12/House-Price-Prediction/blob/main/Images/Price-per-area_outliers.png)
  Rectified Data
  ![Corrected Price/ Sq. foot](https://github.com/Shubhamag12/House-Price-Prediction/blob/main/Images/Corrected_Price-per-area_outliers.png)
  
</details>

<details open>
  <summary>New Features</summary>
  
  All the features provided can be reframed to the format : {Area, AttributeScore, Resale, LogPremium, Bedrooms}
  1. Area = <int> Floor area of the property
  2. AttributeScore = <int> An integer based on features like num of bedrooms, gym facility, etc
  3. Resale = <int> A binary value denoting if the propery is first hand usage (0) or a resale (1)
  4. LogPremium = <int> An integer value depending on the Price per sq. foot value
  5. Bedrooms = <int> Number of bedrooms in the property
</details>

Final Correlation Matrix :
![Plot of Correlation Matrix](https://github.com/Shubhamag12/House-Price-Prediction/blob/main/Images/correlation_matrix.png)

## Model selection
Two models were cosidered as most optimum ones, whose predictions are depicted below:

Ordinary Least Squares | Linear Regressor
------------ | -------------
![OLS Plot](https://github.com/Shubhamag12/House-Price-Prediction/blob/main/Images/ols_model_prediction_plots.png) | ![Linear Regression Plot](https://github.com/Shubhamag12/House-Price-Prediction/blob/main/Images/linear_regression_model_prediction.png)
92.9 (R-squared value) | 81.705317 (Cost)


## Results
The trained OLS model gives an accuracy of 92.9 (R-squared value). The model summary for the same is provided below

![OLS Model Summary](https://github.com/Shubhamag12/House-Price-Prediction/blob/main/Images/OLS_model_Summary.png)
