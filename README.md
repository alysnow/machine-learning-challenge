# machine-learning-challenge - Exoplanet Exploration
Week 21 - Homework

![exoplanets.jpg](Images/exoplanets.jpg)


## Background

Over a period of nine years in deep space, the NASA Kepler space telescope has been out on a planet-hunting mission to discover hidden planets outside of our solar system.

To help process this data, I have created machine learning models capable of classifying candidate exoplanets from the raw dataset.

In this homework assignment, I have completed the following:

1. Preprocess the raw data
2. Tune the models
3. Compared three models

- - -

## Models

* Logistic Regression

* Support Vector Machine

* Random Forest Classifier

- - -


## Resources

* [Exoplanet Data Source](https://www.kaggle.com/nasa/kepler-exoplanet-search-results)

* [Scikit-Learn Tutorial Part 1](https://www.youtube.com/watch?v=4PXAztQtoTg)

* [Scikit-Learn Tutorial Part 2](https://www.youtube.com/watch?v=gK43gtGh49o&t=5858s)

* [Grid Search](https://scikit-learn.org/stable/modules/grid_search.html)

- - -

## Considerations

* Start by cleaning the data, removing unnecessary columns, and scaling the data.

* Not all variables are significant be sure to remove any insignificant variables.

* Make sure your `sklearn` package is up to date.

* Try a simple model first, and then tune the model using `GridSearch`.

- - -

## Assignment structure
```
machine-learning-challenge
|__ .git                                       # Gitignore file
|__ Comparison Model Report.md                 # Markdown Report
|__ README.md                                  # Markdown README
|__
|  |__ data/                                   # JavaScript and CSS Styles directory
|     |__ exoplanet_data.csv                   # Exoplanet csv file
|__
|  |__ Images/                                 # PNG files
|     |__ exoplanets.jpg                       # README png
|     |__ model_results.PNG                    # Results png
|__
|  |__ models/                                 # Model files
|     |__ model_1_LG.sav                       # Logistic Regression Model
|     |__ model_2_SVM.sav                      # Support Vector Machine Model
|     |__ model_3_RF.sav                       # Random Forest Classifier Model
|__
|  |__ notebooks/                              # Jupyter notebook files
|     |__ model_1_LG.ipynb                     # Logistic Regression Model Jupyter notebook
|     |__ model_2_SVM.ipynb                    # Support Vector Machine Model Jupyter notebook
|     |__ model_3_RF.ipynb                     # Random Forest Classifier Model Jupyter notebook

```
- - -

## Usage

```
# Update sklearn to prevent version mismatches
# -------------------------------------------
!pip install sklearn --upgrade

# install joblib. This will be used to save your model. 
# Restart your kernel after installing 
# -------------------------------------------
!pip install joblib

# Dependencies and Setup Jupyter Notebook
# -------------------------------------------
import pandas as pd
from sklearn.model_selection import train_test_split
from sklearn.preprocessing import StandardScaler
from sklearn.linear_model import LogisticRegression
from sklearn.svm import SVC
from sklearn.ensemble import RandomForestClassifier
from sklearn.model_selection import GridSearchCV

```
- - -

## Datasets 

|No|Source|Link|
|-|-|-|
|1|exoplanet_data.csv|https://github.com/alysnow/tableau-challenge/blob/main/data/CitiBike_Complete.csv|

- - -

## Task

### Preprocess the Data

* Preprocess the dataset prior to fitting the model.
* Perform feature selection and remove unnecessary features.
* Use `MinMaxScaler` to scale the numerical data.
* Separate the data into training and testing data.

[Jupyter Notebooks](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html?highlight=random%20forest#sklearn.ensemble.RandomForestClassifier) are available to view in the link provided.

### Tune Model Parameters

* Use `GridSearch` to tune model parameters.
* Tune and compare at least two different classifiers.

[Jupyter Notebooks](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html?highlight=random%20forest#sklearn.ensemble.RandomForestClassifier) are available to view in the link provided.

### Report

A [Comparison Model Report](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html?highlight=random%20forest#sklearn.ensemble.RandomForestClassifier) is avaiable in the link provided.

- - -

## Contributor
- [Alysha Snowden](https://github.com/alysnow)

