# Twitter_Covid19

The main goal is to build a Retweet Prediction Model that predicts how many retweets a tweet will get and shows how different features affect its performance.
In the first part, I did an analysis of the feature in order to understand deeper the dataset. 
In a second part, I adopted different Machine Learning approaches using data related to the author of the tweet, and to the characteristics of the message itself which includes Sentiment Analysis.

<img
src=“word_cloud_tweet.png”
raw=true
alt=“Subject Pronouns”
style=“margin-right: 10px;”
/>

## Feature Engineering

The training dataset we have been provided with contains 665 777 samples of tweets related to COVID-19. 

On top of the features provided by the challenge for each tweet which has been introduced, I extracted more features which are described in detail in Table 1, based on past research in the field, as well as on our intuition, we calculated some extra features which seemed to influence the number of retweets a tweet might get. The features we used for training models and can be classified into four categories: (1) user features, (2) content features, (3) time features, and (4) sentiment features.
We have explored many avenues that may or may not have been used for different reasons. We have listed in this table the different features we have worked with, and whether we have implemented them in our prediction models or not.

## User Feature Related 

User Features : denote a set of features related to the author of a tweet: whether he is verified, how many followers and friends he has, and the total number of statuses he has posted. In addition to the number of followers and friends of a user, I also included the ratio of those two numbers. The total number of tweets shows the activity level of a user and we found that it helped to improve the prediction performance. 
My first hunch was to say that a verified accompt is strongly correlated with getting more retweeting. By a simple visualization we can notice that the rate of people checking who tweet is enormously correlated to the rate of tweeting who have been retweeted.  It is easy to understand that a verified account is more influential, because it is often more followed, and often more influential on public opinion


Taking the example of Donald Trump, a very famous certified Twitter user. 
We notice that these tweets are always retweeted massively, no matter the subject or the connotation of the subject. Let's take the example of 2 of these tweets, one congratulating China and another one blaming it. In both cases the tweet was RT massively. Verified accounts are therefore more often retweeted regardless of the content of the tweet.
By grouping, we can observe that 72% of the tweet from unverified users are not retweeted compared to less than 1% of the tweet from verified users are not retweeted.



## Tweet Related Feature

## Sentiment Analysis
