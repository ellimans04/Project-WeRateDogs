# Project-WeRateDogs
Data Wrangling Report (WeRateDogs)
By Elliot Manuel Sithole
06/09/2022
Context
The project involves the wrangling of data from various sources associated with tweets
from Twitter; WeRateDogs. This rates pictures of dogs in a humorous manner, most
often giving ratings higher than 10/10.
The Objectives
The main objective of this project is to perform data wrangling that is gathering,
assessing and cleaning from three different sources. The focus is on improving and
fixing quality and tidiness issues and then storing, visualising and analysing the
wrangled data to review vital insights.
Step 1:
In this project, all three pieces of data were sourced from three different means and
uploaded into the pandas data frame:
1. Twitter archive file: manual direct download of the file
(https://d17h27t6h515a5.cloudfront.net/topher/2017/August/59a4e958_twitter-archiveenhanced/
twitter-archive-enhanced.csv),
2. The tweet image predictions: the dog breed prediction is present in each tweet
according to a neural network. This file (image_predictions.tsv) is hosted on Udacity's
servers and downloaded programmatically using the Requests library and URL link
(https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_imagepredictions/
image-predictions.tsv).
3. Twitter API & JSON: Data gathered for each tweet's retweet count and favourite
count at a minimum. Using the tweet IDs in the WeRateDogs Twitter archive, to query
the Twitter API for each tweet's JSON data using Python's Tweepy library and to store
each tweet's entire set of JSON data in a file (tweet_json.txt file). Each tweet's JSON
data is written to its line and then read as .txt file line by line into a pandas DataFrame
with (at minimum) tweet ID, retweet count, and favourite count.
Step 2:
Quality
After a thorough visual and programmatic assessment, several issues were
documented, about quality and tidiness shortfalls.
