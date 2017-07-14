# NLP
Use NLP to extract features from bodybuilding.com forum article titles and classify them into 8 muscle groups. Train the data with XGboost and Tensorflow. 

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
- Remove numbers, punctuations, and https://
- TFIDFVectorizer

## Model
- Benchmark : random forest
- XGboost : gradient boosting tree
- Tensorflow NN single layer
- Tensorflow RNN : recurrent neural network

## Required Libraries
- sklearn
- numpy
- pandas
- xgboost
- tensorflow