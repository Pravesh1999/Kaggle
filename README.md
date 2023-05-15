# Sentiment Analysis of COVID-19 Tweets
This notebook aims at building a text classification model using the tweets related to the COVID-19 pandemic which contains about 41157 tweets from twitter users across the globe. When given a tweet the engine cleans the text and tries to classify if the tweet is Positive,Negative,Extremely Positive,Extremely Negative or Neutral.

The DATA folder contains both the training and testing data. Both training and testing data contains the following columns:
  1) UserName : To maintain anonymity of users the usernames have been replaced with a random integer value
  2) ScreenName : This contains the masked screen name to maintain user anonymity
  3) Location : The location from which the tweet has been made from
  4) TweetAt : The date in which the tweet has been made
  5) OriginalTweet : Contains the actual tweet made by the user
  6) Sentiment : This contains the manually labelled sentiment of the tweet

The notebook is organised as follows:
  1) Exploration and EDA of dataset
  2) Text Cleaning:
    2.1) Removing hashtags,RTs,emails
    2.2) Removing URLs
    2.3) Removing punctuation
    2.4) Expainding Text Contractions
    2.5) Removing Numbers
    2.6) Stopword removal
    2.7) Lemmatization
  3) Converting Text into Numerical Representation:
    3.1) TF-IDF vectorization
  4) Building Model:
    4.1) Random Forest
    4.2) Multionmial NB
    4.3) XGBoost
    4.4) LGBClassifier
    4.5) Neural Network
  5) Converting Text into Word Embedding Representation:
    5.1) pre-trained Glove model
