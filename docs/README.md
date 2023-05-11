# DATA_606 - Capstone Project
- Author : Pavani Velma
- Semester : Spring 2023
- Campus ID : vy61891
# Project Title : House Price Prediction Analysis
# Introduction
- Real estate is a crucial sector of the economy.
- Prices of real estate properties such as houses are liked to various factors such as population growth, unemployment, GDP and GNI.
- Accurately estimating the price of houses is essential for a variety of purposes, including buying, selling, investing, and financing.
# Motivation
- As an individual interested in owning a house for myself, I feel there are a lot of things one should take into consideration while buying or selling a piece of property. One of the major things are the finances. It is important have an accurate and realistic price prediction to make a decision on whether or not to buy a house during a specific time or region.
# Objective
- The objective of this project is to 
- To apply data preprocessing and preparation techniques in order to obtain clean data.
- To build machine learning models able to predict house price based on house features
- To analyze and compare models performance in order to choose the best model
# Data Collection
- I have took the 5 datasets for 1 bedroom, 2 Bedroom, 3 bedroom, 4 bedroom, 5 bedroom from kaggle and merged into one Dataset.
- I am using a dataset that has historical date of houses sold in different counties, states in USA across multiple years starting from 1995 to 2020.
- The dataset was obtained from Kaggle.com via the source.
- The output feature is the house price in dollars.
<img width="865" alt="Screen Shot 2023-05-11 at 1 41 28 PM" src="https://github.com/DATA-606-SPRING-2023-THU/pavani_606/assets/99057026/42bb3042-d024-4c29-b960-7c22030910bf">

# Data Cleaning
- Merged multiple datasets.
- Calculated monthly house price into yearly avg price.
- Removed redundant columns.
- Removed rows with null values.
# Exploratory Data Analysis
- But before I start modeling, I need to understand the data and how it is represented in the dataset.
# top five counties with highest average price
- Pitkin county, Colorado, has highest avg house prices since 1996.
- San Mateo county, California, has lowest avg house prices since 1996
# top five counties with highest growth rate
- Gallatin County, Montana, has highest growth rate. House prices in Gallatin County has increased 350 times since 1996.
Heard, Quitman, Hot Spring Counties have similar growth rate.
# Distribution of no.of beds
- Highest number of houses in USA has 3 bedrooms.
- Houses with single bedroom are low in count.
# Correlation with target
- Beds and avg price are highly and positively correlated that means higher the no.of beds higher the price of the house
Size rank is negatively correlated. 
- Lowest size rank has highest price
# Average housing prices 
- From 2006 to 2012  Average price gradually decreased.
- From 2012 Average price increased and peaked at 2019.
- Due to Covid-19, avg prices again decreased.

# Prediction Modelling
- Below selected models has been used for machine learning modelling for k-best features.
- Decision tree
- Random forest regressor
- Linear regression
# Linear Regression
- Linear regression is a type of supervised learning algorithm used in machine learning that helps to predict a continuous output variable based on one or more input variables. The goal of linear regression is to find the best linear relationship between the input and output variables. 
<img width="310" alt="Screen Shot 2023-05-11 at 3 18 27 PM" src="https://github.com/DATA-606-SPRING-2023-THU/pavani_606/assets/99057026/5729ca00-b093-4fc1-b1b7-f9becb9d1c1c">
# Result:
<img width="310" alt="Screen Shot 2023-05-11 at 3 18 58 PM" src="https://github.com/DATA-606-SPRING-2023-THU/pavani_606/assets/99057026/f3cf4be1-d955-4fc3-b5c5-d5630ce93790">











