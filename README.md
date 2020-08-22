# Ford-Used-Car-Predictions


## Table of contents
* [General Info](#general-info)
* [Data](#data)
* [Idea](#idea)
* [Results](#results)

## General Info
The whole data set contains about 370.000 used cars from Ebay-Kleinanzeigen including all kind of brands

## Data
* [Data set](https://www.kaggle.com/orgesleka/used-cars-database)
* The content of the data is in German, but it should also be understandable for non-German speakers

## Idea
* Only keep rows that include Ford cars
* Created a XGBoost Regression Model to predict Ford used car prices based on the reduced data set

## Results
* Mean Absolute Error: 680.63€
* Mean Squared Error: 1296394.66€
* Root Mean Squared Error: 1138.59€
* R2 Score: 94%
