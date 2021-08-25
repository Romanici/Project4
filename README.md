# Sparkify User Churn Prediction

Sparkify is a fictional music streaming platform created by Udacity. For this project we are given log data of this platform as a json file in order to drive insights and create a machine learning pipeline to predict user churn. Any platform is instered in detect which users are likely to cancel the service so as to take action (offer discounts, promotions etc.) to retain them. But you also have to be careful and avoid giving discounts to users that are not actually thinking about leaving the service. 

You can find more information about the project in my post [here](https://medium.com/p/17366df43078/edit).

So, the steps of the project are the following:

- Cleaning the data.
- Exploratory data analysis.
- Feature engineering.
- Modeling.
- Evaluation of the results and discussion.


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
- F1 score, accuracy and training time. Note that the important metric is F1 since we 
<img src="https://github.com/Romanici/Project4/blob/main/results_models.png" width="600">
- ROC curve logistic regression
<img src="https://github.com/Romanici/Project4/blob/main/roc_lr.png" width="600">

The results are reasonably good, the models have notorious predictive value. The f1 score of logistic regression is 0.81, close to the highest possible value of 1.0, which would indicate perfect precision and recall.

## Discussion

A list of things remain to be done. Here I comment just some of them:
- First and the most important one, I still have to process the complete dataset using a Spark's cluster. The results are obtained from a subset of the dataset. 
- Improve tuning of the random forest and gradient boosting, try more hyperparameters. 
- Assess how unbalanced is the data. In practice, during a given period very few users churn with respect to the total population. 
- More careful analysis in the feature engineer step, more features can be created. 

## Acknowledgements

The dataset is provided by Udacity. The project is proposed by Udacity as part of the Udacity Data Scientist Nanodegree Capstone Project.
