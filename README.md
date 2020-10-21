# House-Price-Prediction

## Overview
This is an ML-based application that predicts the house prices based upon the features provided (such as area, num of bedrooms, etc.)

Model Used | Accuracy
------------ | -------------
Linear Regressor | 81.705317 %
Ordinary Least Squares | 92.9 (R-squared value)

File Description:
- **Delhi.csv** : dataset
- **Delhi.ipynb** : Main file with all processing stuff
- **DElhi_load.ipynb** : Application interface for users.

## Problem Statement
Given a set of features, predict the price of any given house in the Delhi region.

## Dataset and libraries used

<details open>
  <summary><b>Dataset Summary</b></summary>
  
  
  1. Reference link for dataset : [click here]()
  2. df.info()
</details>

<details>
  <summary>Libraries Used</summary>
  
  1. Pandas
  2. Statsmodel
  3. Sklearn
  4. Numpy
</details>

## Feature analysis

<details>
  <summary>Outliers</summary>
  
  1. Price
  2. Area
  3. Price per sq. foot
</details>

<details open>
  <summary>New Features</summary>
  
  All the features provided can be reframed to the format : {Area, AttributeScore, Resale, LogPremium, Bedrooms}
  1. Area = <int> Floor area of the property
  2. AttributeScore = <int> An integer based on features like num of bedrooms, gym facility, etc
  3. Resale = <int> A binary value denoting if the propery is first hand usage (0) or a resale (1)
  4. Bedrooms = <int> Number of bedrooms in the property
</details>

Final Correlation Matrix (plot):

## Model selection

## Results
The trained OLS model gives an accuracy of -- . The model summary for the same is provided below
