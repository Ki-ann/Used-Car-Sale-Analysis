# Welcome to car-resale-analysis repository

## About

This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on how car prices are affected by these variables from [dataset](https://www.kaggle.com/austinreese/craigslist-carstrucks-data) (Version 10).  

For detailed walk-through, please view the source code in order from:  

1. Exploratory Data Analysis, [Part 1](1.%20EDA-part1.ipynb) & [Part 2](1.%20EDA-part2.ipynb)
2. [Data cleaning and Feature engineering](2.%20Data%20cleaning%20and%20Feature%20engineering.ipynb)
3. [Machine model exploration](3.%20Machine%20model%20exploration.ipynb)
4. [XGBoost tree](4.%20XGB%20model%20exploration-20220419-103334.ipynb)
5. [Conclusion](5.%20Conclusions.ipynb)

## Problem Definition

**Main problem:** How different variables such as [odometer, year, condition, fuel, title_status, transmission, drive, state, manufacturer] affect the resale price of a car.  
**Subproblem 1:** How do different models (Tree regressor, linear regression, tree classifier) respond to the variables?  
**Subproblem 2:** Does applying feature engineering to the dataset change the way the model respond (Tree regressor, linear regression, tree classifier) to the dataset?  
**Subproblem 3:** Is there a better model (XGBoost) we can use to better predict the price of the car?

## Models Used

1. Linear Regression
2. Tree Regression
3. Tree Classifier
4. XGBoost

## Presentation

The video to the presentation can be accessed on Youtube [here](https://youtu.be/IUqfuVxWN-Q). Slides are also uploaded to the repository for easy viewing.

## Conclusion

1. The dataset provided on kaggle is very dirty in general
    a. Prices contain a lot of erroneous data points
    b. Many missing values in many categorical variables
2. Just fitting the data points into any machine model with this dataset as seen on many kaggle notebooks yields poor results
    a. By performing some feature engineering we are able to utilise some of the variables that have previously low correlation with price.
3. Use of classification (especially XGBoost) can generate better prediction compared to rudimentary models like linear regression and tree classifier.

4. It is possible to predict resale price of the car with even greater accuracy, and more can be explored with other methods such as neural networks

## What did we learn from this project?

- Regression models may not always be the best approach and other models could give rise to a better fit
- XGBoost and the logic behind the model (concepts about Precision, Recall, and F1 Score)
- Feature engineering techniques such as imputation, discretization... (more in the notebooks)
- To not blindly fit dataset into models as some variables can be insanely skewed

## Contributors

- @HiIAmTzeKean (Data cleaning, Machine model,Conclusions)
- @Ki-ann (XGBoost)
- @onghaixiang (EDA)

## References

- <https://www.kaggle.com/austinreese/craigslist-carstrucks-data>
- <https://www.projectpro.io/article/8-feature-engineering-techniques-for-machine-learning/423>
- <https://machinelearningmastery.com/feature-selection-with-real-and-categorical-data/>
- <https://machinelearningmastery.com/gentle-introduction-gradient-boosting-algorithm-machine-learning/>
