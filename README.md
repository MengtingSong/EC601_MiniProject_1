# EC601_MiniProject_1

## How to run our code?
- Firstly, open TravelTweets.py. Replace the consumer_key, consumer_secret, access_token, access_token_secret with yours.
- Run $ python TravelTweets.py;
- Set up Google environment;
- Wait for the process done. You should see a new folder named "result" created containing 25 text files titled with city names;
- After the folder is successfully created, run $ python languageprocess.py;
- Then you will get a text file named "result.txt" containing a list of 10 cities.

## Vision/Goals of the project:
In this project, we want to know about what are the most welcome cities in the US for a short trip by implenmenting analysis of the tweets. We will give a list of cities ranked from the most positive to the most negative (or least positive) in the overall sentiment of all related text tweet content.

## Users/Customers:
The project can benefit anyone who currently has a plan of traveling or want to get information for certain traveling cities in the US. 

It can also provide information to traveling agencies like which cities are most and least welcome to help them design tourism products, for example, they can use this infomation in advertisement or arrange more trips to the most welcome cities.

## User Stories:
I, as a user, want to know what are the most welcome cities in the US for a short trip.

I, as a foreigner newly arrived at the US, want to know that which cities I should start with for traveling so that I can get the best experience within the limited time.

I, as a travelling agnecy, want to know the popularity rank of the popular US cities, so that I can arrange tourism products accordingly.

## Architecture:
![image text](https://github.com/MengtingSong/EC601_MiniProject_1/blob/master/601_mini1_architecture_v2.png)

## Solutions:
Firstly, we want to identify several US cities that may be popular traveling destinations for people. We referred to "The 25 Best U.S. Cities to Spend a Weekend" updated by THRILLIST TRAVEL on 05/07/2019 (https://www.thrillist.com/travel/nation/best-us-cities-to-spend-a-weekend-nashville-austin-charleston-providence) and took the 25 cities as our base city pool.

Then, we extracted tweets including "#travel OR #holiday OR #vacation AND the city name" for each city. Considering we are recommending US cities, we only searched for English tweets and extracted the most popular and also real-time tweets of the first 100 pages, and excluded retweets to avoid redundancy. For the code of Tweets part, we leveraged TweetSearch library for the sake of convenience which is also included in this git project. Then we wrote each city's tweets into reparative text files so that we can process the twitters' sentiment and feeling in their tweets city by city. 

In the language process program, we read the txt file one by one and use the google NLP api to analyze them. After we got the sentiment scores and magnitudes from google services, we rank this data into a list and sorted these cities by considering both the sentiment scores and magnitudes. Finally we save the result into a txt file and display analysis result in a top-down rank.

## Issues:
The biggest issue is the extracted tweets are quite un-organized and contains a lot of unrelated, trivial or misleading information, for example, some tweets are from traveling agencies or advertisers which will bias the final result. Besides, the total amount of tweets data is too small for a reliable result. To solve this problem, getting some priori knowledge of the tweets publishers and trying to eliminate those irrelevant ones out by setting up filters, also running analysis on the tweets of larger amount and over longer period may be helpful.



