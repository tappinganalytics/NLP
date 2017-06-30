# NLP
Use NLP to extract features from bodybuilding.com forum article titles and classify them into 8 muscle groups. Train the data with XGboost model. 

## Data
[bodybuilding](https://bodybuilding.com) web crawler
67k data entries - 440MB

## Muscle groups:
- chest
- biceps
- triceps
- glutes
- back
- leg
- abs
- shoulders

## Pre-process data 
- TFIDFVectorizer
- NLTK

## Model
- Benchmark : random forest
- XGboost : gradient boosting tree

## Required Libraries
- sklearn
- numpy
- pandas
- xgboost