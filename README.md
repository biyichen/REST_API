# Twitter API

#### using the Tweepy library which will make it very easy for us to connect to the API and start streaming the data.
#### The code below is a simple example that allows us to connect to the API and print tweets from our timeline:

```
import tweepy
auth = tweepy.OAuthHandler(consumer_key, consumer_secret)
auth.set_access_token(access_token, access_token_secret)
api = tweepy.API(auth)
public_tweets = api.home_timeline()
for tweet in public_tweets:
    print(tweet.text)
```
