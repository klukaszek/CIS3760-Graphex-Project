# Twitter.py
Module that handles Tweets for our backend API.
       
## Twitter = <class 'src.lib.twitter.Twitter'>
  
Class that handles Tweets. 

### Methods 

**\_\_init\_\_**(self) -> None

Initialize the Tweepy client with a bearer token. Initialize a list meant for storing Tweets.

**emptyList**(self) -> None

Empties the list of Tweets.

**getNumTweets**(self) -> None

Returns the number of Tweets stored in memory.

**getRecentTweets**(self, query: str, limit: str) -> None

Returns a list of recent tweets using the Tweepy API and search queries.

**getTweepyBearerToken**(self) -> str

Get Tweepy bearer token, for testing purposes.

**printTweetList**(self) -> None

Prints all Tweets in memory.

**readFromCSV**(self, filename: str) -> None

Reads Tweets into memory from a supplied CSV file.

**readFromJSON**(self, filename: str) -> None

Reads Tweets into memory from a supplied JSON file.

**writeToCSV**(self, filename: str) -> None

Writes the Tweets in memory to a CSV file.

**writeToJSON**(self, filename: str) -> None

Writes the Tweets in memory to a JSON file.


* * *

Data and other attributes defined here:  

**Tweet** = <class 'src.lib.twitter.Twitter.Tweet'>

Class that represents a Tweet.