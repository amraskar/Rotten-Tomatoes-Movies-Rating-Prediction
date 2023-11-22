# Rotten-Tomatoes-Movies-Rating-Prediction: Project Overview 
* Build a high performing classification algorithm to predict whether a particular movie on Rotten Tomatoes is labeled as 'Rotten', 'Fresh', or 'Certified-Fresh'.
![alt text](https://github.com/amraskar/Rotten-Tomatoes-Movies-Rating-Prediction/blob/430dace40bc7115bd10ca4fbe2df5abf35b86545/Tomatometer%20Status.png "Number of Fresh, Certified Fresh and Rotten Movies")

## Code and Resources Used 
**Python Version:** 3.11  
**Packages:** pandas, numpy, scipy, sklearn, matplotlib, seaborn, xgboost

## Dataset Used 
**From Kaggle:** https://www.kaggle.com/datasets/stefanoleone992/rotten-tomatoes-movies-and-critic-reviews-dataset/data

## Data Cleaning
I needed to clean it up so that it was usable for our model. I made the following changes and created the following variables:

*	Removed columns with high number of null values.
*	Removed rows with null values.
*	Checked for no duplication.
*	Made columns for the number of directors in each movie.
*	Made columns for the number of authors in each movie.
*	Made columns for the number of actors in each movie.

## EDA
* I looked at the distributions of the data.
* Correlation with the target value.
![alt text](https://github.com/amraskar/Rotten-Tomatoes-Movies-Rating-Prediction/blob/0fe1ee5f6fb050cc0d55ca7e352312384de6ab03/Correlation%20Heatmap.png "Correlations")
* The value counts for the various categorical variables.
* I removed Outliers.
* Dealing with skewed data.
![alt text](https://github.com/amraskar/Rotten-Tomatoes-Movies-Rating-Prediction/blob/aa4e96b3d60070abde4ec76c5acee00a9fd3ef44/Distribution.png "Distributions")

## Model Building 

* First, I transformed the categorical variables into dummy variables.
* I scaled the data using StandardScaler()
* I also split the data into train and tests sets with a test size of 20%.   
   

**I tried three different models:**
* Decision Tree Model
* Random Forest Model
* XGBoost Model 
