#  Web APIs & NLP Project
![alt text](https://storage.googleapis.com/kaggle-datasets-images/2050/3494/c0a4b38eef8ed520bf67f79a22739ba3/dataset-cover.jpg)

# Problem Statement
Our company wants to developed an NLP app which is able to distinguish between news and normal chat. For developing the app, We will train a classification model which will predict between subreddits WorldNews and CasualConversation for a given text.

# Executive Summary
Out of all the classification models built, GaussianNaive Bayes with Word2Vec pre-processing was selected as it achieved the highest PR AUC score of 0.98 on the cross valudation set , outperforming the baseline score of 0.46. Based on intepretation of the model, the model has made sensible prediction on why it classify a text to be a subreddit.

Hence with this, we will be able to use this model for developing the NLP app.


# Evaluation metric
Our company cares more on predicting worldnews (target) and have low false positive rate (high precision) for the NLP app.

Hence we will be using PR-AUC for our evaluation metrics

#Pre Processing
We have investigated pre-processing using 3 methods as below:-
Count Vectorizer
TFIDF Vectorizer
Word2Vec

#Model Fitting
We have fitted 3 models
-Random Forest
-Logistic Regression
-Naive Bayes (Gaussian & Multinomial)

#Conclusion & Future Recommendation
We selected the Naive Bayes Model with word2vec pre-processing as  the best performing model where it has F0.5 scores of 0.96. We have achieve a metric score significantly higher than our baseline 0.46, and based on the model interpretation we are confidence that it will generalize.

In future, we can add Topic modelling to generate insights of what are the subject being discussed in both subreddits.

## Content
- [Data Description](#Data-Description)
- [Evaluation Metric](#Evaluation-Metric)
- [Executive Summary](#Executive-Summary)
- [Imports](#Imports)
- [Text Cleaning](#Text-Cleaning)
- [Exploratory Data Analysis](#Exploratory-Data-Analysis)
- [Preprocessing](#Preprocessing)
    - [Count Vectorizer](#CountVectorizor)
    - [TFIDF Vectorizor](#TFIDF-Vectorizor)
    - [Word2Vec](#Word2Vec)
- [Model Fitting](#Model-Fitting)
    - [Random Forest](#Random-Forest)
    - [Logistic Regression](#Logistic-Regression)
    - [Naive Bayes](#Naive-Bayes)
- [Model Comparison & Selection](#Model-Comparison-&-Selection)
- [Model Interpretability](#Model-Interpretability)
- [Conclusion & Future Recommendation](#Conclusion-&-Future-Recommendation)
