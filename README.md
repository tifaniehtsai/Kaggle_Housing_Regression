# House Prices - Advanced Regression Techniques 
This project focuses on predicting housing prices using the LASSO (Least Absolute Shrinkage and Selection Operator) regression technique. 

## Dataset
Competition Link: [Kaggle Competition Link](https://www.kaggle.com/competitions/house-prices-advanced-regression-techniques/data?select=test.csv)
Dataset: consists of training and test sets, containing information about residential properties. 
Features: square footage, number of bedrooms and bathrooms, location, and other attributes. 
Goal: build a predictive model that best estimates the sale prices of houses based on the features

## Techniques
- EDA to understand the distribution of features and relationship with the target variable
- Visualizations such as histograms, heatmaps, and scatter plots
- Feature Engineering to improve model performance
- LASSO regression

## In Depth Approach
1) Data Processing:
    - focused on removing outliers first, did some EDA such as plotting a scatterplot of GrLivArea (ground living area square feet, chose this feature because highest numerical correlation to target) against SalePrice (target)
    - dropped unnecessary columns such as Utilities
    - impute nulls for Bsmt and Garage features as well as other features such as fireplace, fence, alley
2) Feature Engineering:
    - created new features such as AgeHouse, TotalSF, TotalBsmt, TotalBath as well as binary features such as HasBasement
3) Data Processing Part 2:
    - transformed numerical features using Log1p
    - encoded categorical features
4) LASSO Regression
    - LASSO Regression performs feature selection and regularization, which is effective for this type of data
5) Prediction
    - generated predictions for test set
    - result: score = .12993, 910/4549 entries (20%)


## Dependencies
- Python
- Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn
