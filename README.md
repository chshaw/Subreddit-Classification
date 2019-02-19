
# Project 2: Reddit NLP Classification


## Problem Statement

What is the best model to classify which subreddit a post originated from?

## Executive Summary

Using different count vectorizors, the best way to classify where a reddit post originated was to use a logistic regression with the TF-IDF vectorizer with some tuned parameters.

### Contents:
- [Data Dictionary](#Data-Dictionary)
- [Conclusions and Recommendations](#Conclusions-and-Recommendations)

## Data Dictionary

|Feature|Type|Dataset|Description|
|---|---|---|---|
|subreddit|int|created|subreddit where 1 is politics and 0 is scifi| 
|title|string|created|title of the subreddit post| 

## Conclusions and Recommendations

The best way to predict whether a post was from the politics subreddit or the scifi subreddit was by vectorizing the posts with the TF-IDF vectorizer, with n-grams from 1 to 10 and a maximum amount of features of 5,000.  Once the posts were vectorized, the most accurate model was logistic regression with a .976 on the train set and .965 on the test set.
