# Predicting-Survivors

## Introduction
In this repository I illustrate my first foray into machine learning using the [titanic dataset](https://www.kaggle.com/c/titanic/data) from Kaggle. This is a wellknown introductory dataset for those interested in data science and challenges the student to predict who will survive the Titanic using a number of explanatory variables. For my analysis I chose to logistic regression as the classifier and after data cleaning and feature selection wound up with an AUC score of 0.87. The repository contains the Jupyter notebook I used in my analysis.

## Overview
The biggest hurdle I faced for this dataset was filling the null values for age. I wound up comparing two methods: one which filled using the median of the entire age column and one which used the median based on class, age and title. Both methods resulted in the same AUC score of 0.87. Additionally I did some feature engineering by including a new "Titles" column and a "Has Cabin" column.

### Dependencies:
1. [Pandas](http://pandas.pydata.org/)
2. [Seaborn](https://seaborn.pydata.org/)
3. [Matplotlib](https://matplotlib.org/)
4. [NumPy](http://www.numpy.org/)
5. [SciKit-learn](http://scikit-learn.org/stable/)

### Outline of Notebook:
1. Introduction
2. Summarizing the Data
3. Examining relationship with Outcome Variable
4. Cleaning data
5. Creating model
6. Evaluation model
7. Future directions
