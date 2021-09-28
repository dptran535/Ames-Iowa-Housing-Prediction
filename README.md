## Dennis Tran, DSI-Deckard

## Instructors: Gwen Rathgeber, Heather Robbins, Anderson Prewitt

## Problem Statement

Prospective home buyers may not be aware of the factors that contribute to home sale price.

We wish to discover attributes that contribute to the pricing of homes in Ames, Iowa, and create a model that could predict the sale price.

## Executive Summary

To achieve our goal, we found we cleaned our data, performed some exploratory data analysis, and used three regression methods on our data to create our model.

We cleaned our data with the following:
1. We combined our training and testing data together for ease of cleaning and for potential feature transformations.
2. We found null values and filled them in according to the following:
    2a. For values where a null value indicated the lack of an feature, we imputed 0 for numeric columns and None for object columns.
    2b. Garage Year Built was imputed with Year Built
    2c. Other nulls were replaced with either the median or mode depending on the column.

We explored and visualized our data with the following:
1. Calculated the correlation of numeric columns with Sale Price.
2. Examined Overall Quality and Condition of houses.
3. Plotted Neighborhoods and their corresponding Sale Prices
4. Plotted the Year Built of houses and their Sale Price

Then we created our models:
1. A Linear Regression with our numeric columns
2. A Ridge Regression with our numeric columns and some categorical features.
3. A Lasso Regression with the same data from number 2.
4. Our Linear Regression model was the best performing with an R2 of 87%.

## Conclusions and Recommendations

For the potential home buyer, house prices can be determind by examining the size of the property. If the the sheer square footage is higher, it will most likely have a higher price. The overall quality is a given as well. Homes that have higher qualities in their Kitchen and Exterior will have a greater value. Not only that, but the neighborhood a house is located in will also have an effect on the price. Modern homes are valued more than older homes in general. This could be due to factors outside the data provided, such as an increase in Real Estate investment.

In sum, the potential home buyer should be on the look out for when the house was built, where the house is located, how large the house is, and of what quality the home is to determine the possible sale price.

Our model was able to explain about 87% of the variability in sale price of the training dataset. It is a decent predictor of Sale Price Ames, Iowa.

## Sources

1. [Kaggle Competition](https://www.kaggle.com/t/060ea4ec8c78458698c7f9b7e40a00d1)
2. [Ames Housing Data](http://jse.amstat.org/v19n3/decock/DataDocumentation.txt)


## Data Dictionary

For the complete dictionary, please visit the 2nd link in Sources.