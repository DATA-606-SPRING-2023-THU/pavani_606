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

![image0](https://github.com/DATA-606-SPRING-2023-THU/pavani_606/blob/main/docs/Images/Top%20priced%20Houses%20in%20CountyName%2C%20State.png)


- Pitkin county, Colorado, has highest avg house prices since 1996.
- San Mateo county, California, has lowest avg house prices since 1996
# top five counties with highest growth rate

![image4](https://github.com/DATA-606-SPRING-2023-THU/pavani_606/blob/main/docs/Images/Top%205%20Counties%20with%20Highest%20Growth%20Rate%20in%20House%20Prices.png)


- Gallatin County, Montana, has highest growth rate. House prices in Gallatin County has increased 350 times since 1996.
Heard, Quitman, Hot Spring Counties have similar growth rate.
# Distribution of no.of beds

![image1](https://github.com/DATA-606-SPRING-2023-THU/pavani_606/blob/main/docs/Images/Distribution%20of%20Number%20of%20Beds.png)

- Highest number of houses in USA has 3 bedrooms.
- Houses with single bedroom are low in count.

# Correlation with target
![image2](https://github.com/DATA-606-SPRING-2023-THU/pavani_606/blob/main/docs/Images/Correlation%20with%20Target.png)

- Beds and avg price are highly and positively correlated that means higher the no.of beds higher the price of the house
Size rank is negatively correlated. 
- Lowest size rank has highest price

# Average housing prices 

![image3](https://github.com/DATA-606-SPRING-2023-THU/pavani_606/blob/main/docs/Images/AveragePrice_TimeChart.png)

- From 2006 to 2012  Average price gradually decreased because there's a decrease in GDP,GNI and increase in unemployment. 
- From 2012 Average price increased and peaked at 2019.
- Due to Covid-19, avg prices again decreased.
#### Since GDP, GNI and unemployement affects house prices, I have included GDP, GNI, population and unemplyement rates for my analysis. 

# Prediction Modelling
- Below selected models has been used for machine learning modelling for k-best features.
- Decision tree
- Random forest regressor
- Linear regression

# Linear Regression
- Linear regression is a type of supervised learning algorithm used in machine learning that helps to predict a continuous output variable based on one or more input variables. The goal of linear regression is to find the best linear relationship between the input and output variables. 

![image5](https://github.com/DATA-606-SPRING-2023-THU/pavani_606/blob/main/docs/Images/LinearRegression.png)

Result:

![image6](https://github.com/DATA-606-SPRING-2023-THU/pavani_606/blob/main/docs/Images/LinearRegression_Scores.png)


# RandomForest Regressor
- Random forest regressor is a supervised learning algorithm used in machine learning for regression problems. It is an extension of the decision tree algorithm that uses an ensemble of decision trees to improve the accuracy and reduce the overfitting problem.
- The trees in random forests run in parallel, which means there is no interaction between these trees while they are being built.

![image7](https://github.com/DATA-606-SPRING-2023-THU/pavani_606/blob/main/docs/Images/RandomForestRegressor.png)


Result:

![image8](https://github.com/DATA-606-SPRING-2023-THU/pavani_606/blob/main/docs/Images/RandomForest_scores.png)

# DecisionTree
- Decision tree regressor is a supervised learning algorithm used in machine learning for regression problems.
- The decision tree is built by recursively partitioning the input space based on the values of the input features. The algorithm selects the feature and threshold that results in the greatest reduction in the mean squared error (MSE) of the output variable. 
- This process continues until a stopping criterion is met, such as reaching a maximum depth, or a minimum number of samples in a leaf node.

![image9](https://github.com/DATA-606-SPRING-2023-THU/pavani_606/blob/main/docs/Images/DecisionTreeREgressor.png)

Result:

![image10](https://github.com/DATA-606-SPRING-2023-THU/pavani_606/blob/main/docs/Images/DecisionTree_Scores.png)

# Conclusion
- I have trained 3 models such as linear_regression, decision_tree, random_forest,and we can see that the best performing model is decision_tree.
- The mean absolute percentage error for the model is 0.23 and 0.31 for train and test respectively whereas the r2 scores are 0.73 and 0.56 respectively for train and test.
- I have used monotone to make sure the features which is correlated to the input and has an impact should affect during the model building.
- Linear models such as RandomForest and LinearRegression are also performing well, but not able to capture the pattern and generating less r2 score. Also, the percentage error is very high as compared to other models.
# Reference

- Bedrooms dataset

https://www.kaggle.com/datasets/paultimothymooney/zillow-house-price-data?resource=download&select=State_Zhvi_1bedroom.csv

- GDP dataset:
https://www.thebalancemoney.com/us-gdp-by-year-3305543

- GNI dataset:
https://www.macrotrends.net/countries/USA/united-states/gni-gross-national-income

- UnEmployement dataset:
https://data.bls.gov/timeseries/LNS14000000

- population dataset:
https://www.census.gov/data/tables/time-series/demo/popest/2020s-state-total.html

### Links:
#### Presentation links:
- [Youtube](https://youtu.be/vwrJeSaHYuQ)
- [Powerpoint presentation](https://github.com/DATA-606-SPRING-2023-THU/pavani_606/blob/main/docs/Presentation%202.pptx)










