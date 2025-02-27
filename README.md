# Worker-Absenteeism-Classification
This project builds a classification pipeline to predict the amount of time a worker will be absent from work based on their characteristics and the specifics of the missed work day. The target variable, TimeOff, has four categories:

Low

Medium

High

Very High

The project leverages both deep learning (a neural network) and traditional machine learning approaches to address the classification task.

## Overview
The objective of this project is to:

Preprocess and clean a dataset containing worker characteristics and work absence data.
Handle missing values and perform feature engineering (e.g., label encoding for categorical variables).
Split the data into training, validation, and test sets (with optional stratified splitting to maintain class balance).
Build and evaluate a neural network model with hyperparameter tuning.
Visualize training progress using loss and accuracy plots.


## Data
Data Source: time_off_data_train.csv

Features: Worker characteristics (e.g., Reason, Month, Day, Transportation expense, Residence Distance, Service time, Education, Son, Smoker, Pet, Weight, Height, Season, Drinker, Age Group)

Target: TimeOff (4-class categorical variable)

Note: The dataset contains missing values, which are handled by filling numerical features with the mean and categorical features with the most frequent value or a specified placeholder.


## Model Performance 
**IMPORTANT INFORMATION** : A random guess in this case would give us 25%, as there are 4 different classes we trying to predict.

To be honest, the results are pretty bad. The best result I achieved was 53% accuracy using a neural network, and that came only after many experiments and trying various approaches. After analyzing the data and testing different techniques, I concluded that the data itself lacks clarity, making it difficult for the algorithms to identify meaningful patterns. This suggests that further investigation into data quality, preprocessing, and feature engineering is necessary to improve model performance.
Anyways most of the algorithms reached about 40-50% accuracy, with NN hitting 53% which was the best.
