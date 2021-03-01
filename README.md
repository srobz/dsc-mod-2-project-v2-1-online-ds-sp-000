# Module 2 Final Project

## Introduction

The purpose of this project was to clean, organize, and analyze a datset about houses with a multivariate linear regression in order to predict the sale prices of homes with certain attributes.

## Process

1. Data Preparation
2. Data Exploration
3. Data Modeling/Validation

## Exploratory Data Analysis

The questions that are answered throughout this project are:

1. What features have the highest correlation with price?
2. Does grade vary by location?
3. Is the number of bathrooms or number of bedrooms more important?


### 1.What features have the highest correlation with price?
It was determined that grade (house rating), latitude, and bathrooms have the highest correlation with price. Using just these features to make a quick model, it appears as though they can explain approximately 54% of our price data.
![graph](https://raw.githubusercontent.com/srobz/dsc-mod-2-project-v2-1-online-ds-sp-000/master/Visualizations/FeaturesImpactingPrice.png)


### 2. Does grade vary by location?
Mapping out the grade variations by location (using longitude and latitude) was helpful in visualizing the spread of houses but there was no discernible pattern to the spread; there were mainly clusters of similarly graded houses surrounded by clusters of other similarly graded houses.
![graph](https://raw.githubusercontent.com/srobz/dsc-mod-2-project-v2-1-online-ds-sp-000/master/Visualizations/GradeVaryLocation.png)


### 3. Is the number of bathrooms or number of bedrooms more important?
In order to determine if bathrooms or bedrooms were important, I created a graph to visualize the spread, however the graph did not help indicate one over the other. I individually modeled each feature to see which explains more of the data. It was determined that bathrooms are more important, as they explain aproximately 18% of our price data while bedrooms only explain approximately 8.2% of our price data.
![graph](https://raw.githubusercontent.com/srobz/dsc-mod-2-project-v2-1-online-ds-sp-000/master/Visualizations/BathroomsVsBedrooms.png)


## Model Validation

Three models were made prior to model validation. Model 1 removed features with p-values greater than 0.05. Model 2 removed features with variance inflation factors that were significantly higher than the rest. Model 3 removed features with p-values greater than 0.005.

Both the training set and test set yielded an R-squared of approximately 0.456.

## Features Impacting Price

Below are the three features that have the highest impact on price; grade, floors, and bathrooms.

- Grade: Grade, which we can think of as a house rating, has the biggest impact on price. When everything else is held constant, you can expect a price increase of about $112,000 per additional point.
- Floors: The number of floors in the home can vastly change the price as well; specifically between 2.0 and 2.5 floors. When everything is held constant, houses wit 2.5 floors cost about $95,000 more than houses with 2.0 floors.
- Bathrooms: The number of bathrooms the home has can also affect the house price. When everything is held constant, for eacha dditional bathroom the house has you can expect a price increase of about $12,000.


## Repository Organization

- ['Module 2 Project - 1. Data Preparation.ipynb'](https://github.com/srobz/dsc-mod-2-project-v2-1-online-ds-sp-000/blob/master/Module%202%20Project%20-%201.%20Data%20Preparation.ipynb) : Jupyter notebook of Data Preparation with code and comments
- ['Module 2 Project - 2. Data Exploration.ipynb'](https://github.com/srobz/dsc-mod-2-project-v2-1-online-ds-sp-000/blob/master/Module%202%20Project%20-%202.%20Data%20Exploration.ipynb) : Jupyter notebook of Data Exploration with code and comments
- ['Module 2 Project - 3. Modeling.ipynb'](https://github.com/srobz/dsc-mod-2-project-v2-1-online-ds-sp-000/blob/master/Module%202%20Project%20-%203.%20Modeling.ipynb) : Jupyter notebook of Modeling with code and comments
- [Module 2 Presentation.pdf](https://github.com/srobz/dsc-mod-2-project-v2-1-online-ds-sp-000/blob/master/Module%202%20Presentation.pdf) : Project presentation
- ['Visualizations'](https://github.com/srobz/dsc-mod-2-project-v2-1-online-ds-sp-000/tree/master/Visualizations) : Folder containing graphs used in presentation and ReadME
- [README.md] : ReadMe
