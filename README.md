# NLP
Use NLP to extract features from EXRX.net exercise information and classify them into 8 muscle groups. Train the data with XGboost, Word2Vec, and Tensorflow. 

## Data
[bodybuilding](https://bodybuilding.com) web crawler
67k data entries - 440MB
[exrx](http://www.exrx.net) web crawler
308 data entries - 360kB


## Muscle groups:
- Chest
- Biceps
- Triceps
- Glutes
- Back
- Leg
- Abs
- Shoulders

## Pre-process data 
- Remove numbers, punctuations, and https://
- TFIDFVectorizer

## Model
- Benchmark : random forest
- XGboost : gradient boosting tree
- Tensorflow NN single layer
- Tensorflow RNN : recurrent neural network
- Word2Vec: gensim word2vec model

## Required Libraries
- sklearn
- numpy
- pandas
- xgboost
- tensorflow
- json
- gensim

## Result

Bodybuilding.com data are too generic for training purpose, we opted to use EXRX.net data. Tensorflow Neural Net gives 93% accuracy within its data set. We need to expand our model to predict potential user question and classify them into 8 categories. For this we use Word2Vec model for calculating the similarity between question sentence and muscle names. The accuracy so far is unclear. 