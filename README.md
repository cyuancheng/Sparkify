# Sparkify

### Chiyuan Cheng 08/23/2019

## Table of Contents

- [Project Motivation](#motivation)
- [Files Description](#description)
- [Results](#results)
- [Software Installation](#installation)
- [Acknowledgements](#credits)



<a id='motivation'></a>
## 1. Project Motivation

The motivation of this project is to use Spark to
- Perform the Exploratory Data Analysis (EDA) with large dataset.
- Perform the Machine Learning with Spark including Feature Engineering, Model Training, Hyperparameter Tuning.

Specifically, Spark was used to manipulate large datasets to engineer relevant features for predicting churn, and also to build machine learning models with pySpark, which is far beyond what could be done with non-distributed technologies.

<a id='description'></a>
## 2. Files Description

The Sparkify_test.ipynb notebook contains all steps in this project.

The data file (medium-sparkify-event-data.json) was downloaded from [Udacity website](https://s3.amazonaws.com/video.udacity-data.com/topher/2018/December/5c1d6681_medium-sparkify-event-data/medium-sparkify-event-data.json).

This data set is a medicum subset (231.4MB) of the full dataset available (12GB). The data file is too large to be included on github.

<a id='results'></a>
## 3. Results

1. There are noticable differences between a paid/free user, song length, total song, lifetime for subscription when comparing users who are churned and remain in service where:

- Free users have a much higher ratio to be churned
- Churn usually happens when a customer subscribes less length of song and listens less song.
- Churned customers usually use the service for a shorter period of time

2. While three models are used to trained the data, Random Forest has a much better performance (with accuracy of 0.83 and F1 score of 0.80) and faster computation time. 

The detailed findings can be found in a blog post available [here](https://medium.com/@cyuancheng/use-machine-learning-to-predict-customer-churn-9281cc249c7a).

<a id='installation)'></a>
## 4. Software Installation

- pyspark 2.4.3
- pandas 0.24.1
- matplotlib 3.0.2
- seaborn 0.9.0

<a id='credits)'></a>
## 5. Acknowledgements

Dataset used in this project was downloaded from the Data Science Capstone Project:Using Spark to Predict Churn with Insight Data Science of the Data Scientist Nanodegree Program. The credit is given to Udacity for the data and instruction.
