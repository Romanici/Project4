# Sparkify User Churn Prediction

Sparkify is a fictional music streaming platform created by Udacity. For this project we are given log data of this platform in order to drive insights and create a machine learning pipeline to predict user churn. 

You can find more information about the project in my post [here](https://medium.com/p/17366df43078/edit).


## Overview

## Requisites

### Dependencies
- Python (3.8)
- Pyspark sql and ml
- Numpy
- Pandas
- Seaborn
- Matplotlib
Other minor libraries are re, copy, time and datetime

### File description
First install all the necessary packages stated in Dependencies.
Run the commands below in your working directory to open the project in jupyter lab:
```
git clone https://github.com/Romanici/Project4.git

jupyter lab
```
Open **Sparkify.ipynb** and run the cells. 


## Results

Some of the results obtained in a first small subset of the data are the following:
- F1 score
- ROC curve logistic regression
- Feature importance of the RF features

## Discussion

A list of things remain to be done. Here I comment just some of them:
- First and most important, use the complete dataset through a Spark's cluster.
- Improve tuning.
- Assess how unbalanced is the data .
- More careful analysis in the feature engineer are, more features can be created. 

## Acknowledgements

The dataset is provided by Udacity. The project is proposed by Udacity as part of the Udacity Data Scientist Nanodegree Capstone Project.
