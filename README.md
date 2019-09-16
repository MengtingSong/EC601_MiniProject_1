# EC601_MiniProject_1

## User Stories
We came up with 6 user stories for now and will select one later:
* I, as an airplane company/travel agency, wants to know what are the top 20 popular travelling cities recently.
* I, as a car manufacturer, wants to know what are the 10 most and 10 least popular cars and top 10 factors twitter users * I, as Coca-Cola or any other company, wants to know the top 20 keywords that people are also talking about when they are talking about Coca-Cola/or other brand.
* I, as a sports club manager, wants to know the popularity of each sports star in my club and be able to know the amount I should prepare for different star’s peripheral products.
* I, as a cell phone product manager, wants to know the new features of our software or hardware are beloved by customers or not, so we can decide whether we keep or abandon the new feature in our next product.
* I, as a government official, wants to know the public sentiment fluctuation after some public emergency happened and it can help me to make the responses or take some action in the right time.
  
## Architecture:
A high-level architecture structure of this project:
![image text](https://github.com/MengtingSong/EC601_MiniProject_1/blob/master/601_mini1_architecture_v1.png)

## Twitter Frameworks (Mengting)
The Twitter part will be completed via using the "TwitterSearch" (and other) library to call the "Search Tweets" API with certain keywords. Useful links are listed as below:

Twitter libs (Python):
https://developer.twitter.com/en/docs/developer-utilities/twitter-libraries
TwitterSearch: This library allows you easily create a search through the Twitter API without having to know too much about the API details. Based on such a search you can even iterate throughout all tweets reachable via the Twitter Search API. 
https://github.com/ckoepp/TwitterSearch

Useful APIs:
GET trends/place: Returns the top 50 trending topics for a specific WOEID, if trending information is available for it. (Or GET trends/closest)
https://developer.twitter.com/en/docs/trends/trends-for-location/api-reference/get-trends-place
Search Tweets: This search API searches against a sampling of recent Tweets published in the past 7 days. Part of the 'public' set of APIs.
https://developer.twitter.com/en/docs/tweets/search/guides/standard-operators

Response format

## Google Frameworks (Shiyang)

Setting up the development environment:
https://cloud.google.com/python/setup

How-to Guides:
  https://cloud.google.com/natural-language/docs/how-to
  Including four functions:
  Analyzing Sentiment
  https://cloud.google.com/natural-language/docs/analyzing-sentiment
  Analyzing Entities
  https://cloud.google.com/natural-language/docs/analyzing-entities
  Analyzing Entity Sentiment
  https://cloud.google.com/natural-language/docs/analyzing-entity-sentiment
  Analyzing Syntax
  https://cloud.google.com/natural-language/docs/analyzing-syntax
  Classifying Content
  https://cloud.google.com/natural-language/docs/classifying-text

Analysis Tutorial
  https://cloud.google.com/natural-language/docs/sentiment-tutorial
