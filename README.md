# Data Analyst Salary Predictions USA

![GitHub repo size](https://img.shields.io/github/repo-size/rm-kara/Data-Analyst-Salaries-Predictions)
![GitHub stars](https://img.shields.io/github/stars/rm-kara/Data-Analyst-Salaries-Predictions)
![GitHub contributors](https://img.shields.io/github/contributors/rm-kara/Data-Analyst-Salaries-Predictions)
![GitHub forks](https://img.shields.io/github/forks/rm-kara/Data-Analyst-Salaries-Predictions)


## Table of contents
* [Project Overview](#project-overview)
* [Getting Started](#getting-started)
    - [Prerequisites](#prerequisites)
    - [Installing Requirements](#installing-requirements)
* [EDA Highlights](#eda-highlights)
* [Tested Model](#tested-model)
* [Model Performance](#model-performance)
* [Resources](#resources)


## Project Overview
In this project I analyzed a dataset containing **over 2000 job advertisements for numerous data analyst positions**.  
The data was cleaned using **Pandas** and **Numpy**, visualizations were developed with **Seaborn** and **Matplotlib**.  
Transformational steps such as encoding categorical- and numerical variables were implemented by using Scikit-learn's **Pipeline** module.  
To narrow down a large hyperparameter space of the developed **RandomForest** model, I used **RandomizedSearchCV**.  
Finally I optimized the model using **GridSearchCV**.

## Getting Started

### Prerequisites
**Python Version:** 3.7  
**Packages:**
* pandas 1.1.0 
* numpy 1.19.1
* scikit-learn 0.23.2
* matplotlib 3.3.1
* seaborn 0.10.1

### Installing Requirements
To create a new anaconda environment, download [conda_requirements.txt](https://github.com/rm-kara/Data-Analyst-Salaries-Predictions/blob/master/conda_requirements.txt) and enter the following command:  
```
<conda create --name <env> --file conda_requirements.txt>
```
To install the packages with pip, download [requirements.txt](https://github.com/rm-kara/Data-Analyst-Salaries-Predictions/blob/master/requirements.txt) and enter the following command:  
```
<pip install -r requirements.txt>
```
## EDA Highlights
**Min- Max- and AVG Salary Distributions:** 
![alt text](https://github.com/rm-kara/Data-Analyst-Salaries-Predictions/blob/master/img/charts/Salary-Distribution.png "Salary Distributions")
***
**Frequency of Skills in the Job Description:**
![alt text](https://github.com/rm-kara/Data-Analyst-Salaries-Predictions/blob/master/img/charts/Important-Skills.png "Analyst Skills")
***
**AVG Salary based on Job Experience:**
![alt text](https://github.com/rm-kara/Data-Analyst-Salaries-Predictions/blob/master/img/charts/Salary-Job-Experience.png "Salary Job Exp")
***
**AVG Salary in different Sectors:**
![alt text](https://github.com/rm-kara/Data-Analyst-Salaries-Predictions/blob/master/img/charts/Salary-Sectors.png "Salary Sectors")
***
**Number of Job advertisements per State:**
![alt text](https://github.com/rm-kara/Data-Analyst-Salaries-Predictions/blob/master/img/charts/Job-Offer-Locations.png "Job offer Locations")

## Tested Model
* RandomForestRegressor

## Model Performance
**Result without model tuning:**
* Before RandomizedSearchCV & GridSearchCV: 21113.82$  

**Results of the final model with tuned Hyperparameters:**
* Best Model's average MAE: 14487.95$

## Resources
* Link to Data: 
    - [Kaggle Dataset](https://www.kaggle.com/andrewmvd/data-analyst-jobs?select=DataAnalyst.csv)
