# TwitterSentimentAnalyzer
Project gives a wordcloud of tweets about Russia-Ukraine war
Program retrieved from : https://thecleverprogrammer.com/2022/03/15/ukraine-russia-war-twitter-sentiment-analysis-using-python/
The data used for this program found here : https://www.kaggle.com/datasets/towhidultonmoy/russia-vs-ukraine-tweets-datasetdaily-updated

Dataset contains tweets regarding Russia and Ukraine from 21 Feb until date. Updated daily. The program uses a downloaded file but can be changed later to automatically fetch the most recent data.

The program  makes a wordcloud of the tweets. We use it for seeing what the positive and negative tweet 'clouds' may look like.
![image](https://user-images.githubusercontent.com/39655509/179661553-9304c4be-f250-4e3c-bf2b-8be3ef4072d5.png)

We use the re library to strip the tweets of all words we don't care about along with punctuation and links. 

To calculate the sentiment scores of the tweets we use the 'vader_lexicon' and make an instance of SentimentIntensityAnalyzer()



This program uses the following imports 
___
import pandas as pd

import seaborn as sns

import matplotlib.pyplot as plt

from nltk.sentiment.vader import SentimentIntensityAnalyzer

from wordcloud import WordCloud, STOPWORDS, ImageColorGenerator

import nltk

import re

from nltk.corpus import stopwords

import string


