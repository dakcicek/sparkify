# Udacity - Sparkify Project

This project is the Udacity Capstone project.

The aim of this notebook is, using Spark framework, to predict churner of audio streaming platform, Sparkify. This is a capstone project for the Udacity data scientist nanodegree program.
Before modelling, I did some feature engineeering. 
First, I have cleaned the columns and transformed some of them for example ts column.
I have generated transaction_timestamp column from ts column to able to understand and use easily.
I have generated registration_timestamp column from registration column to able to understand and use easily.
Then, I have aggregated based on userId, year, month, day
After that finally, I have aggregated data based on only userId column and generated 2 month avg, sum, max, min columns 

Read more here: https://medium.com/@dakcicek/capstone-sparkify-project-2763ea2b9aaa

### Results Summary

After testing different machine learning classifiers with default parameteres, I got following scores : Accuracy: 0.70, F1 Score:0.69 
Decided to select LogisticRegression in order to tune. After fine-tuning parameters (using a grid search with a random forest classifier and logistic regression ), we could improve this to Accuracy: 0.76, F1 Score:0.70


### Files

The only included files are the two notebooks:

1. Sparkify_Exploratory_Data_Analysis.ipynb : This notebook only includes exploratory data analysis part, and data visualization part
2. Sparkify.ipynb : This notebook includes feature engineering and modelling part.

### Requirements

- pyspark
- seaborn
- pandas
- matplotlib

