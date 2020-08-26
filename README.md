## twitter_hashtag
# fetching top 10 hashtag based on retweets

## use your twitter api credientials
consumer_key = **'add your consumer_key'**<br>
consumer_secret = **'add your consumer_secret'**<br>
access_token = **'add your credientials'**<br>
access_token_secret = **'add your credientials'**<br>

## if you want to fetch more than one days tweets change delta value
dt = date.today() - **timedelta(1)**

## if you want to search another hashtag insted of #corona then replace '#corona' string and place new query
for tweet in tweepy.Cursor(api.search,q=**"#corona"**,count=2,since=dt)

## if you want to fetch more number of tweets then increase count value
tweepy.Cursor(api.search,q="#corona",**count=2**,since=dt)
