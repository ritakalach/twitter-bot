# Twitter Bot 🐦🤖 
Automate tweets with tweepy.

## Functions
* ```request_user_input()``` - Type one of the following in the command line: tweet, shuffle quotes, add quote, or exit.
* ```shuffle_quotes()``` - Shuffles quotes currently stored in text file. (I sometimes do this after adding a lot of new quotes from the same book.)
* ```is_file_empty(lines)``` - Takes lines as input; returns True if there are no lines (meaning quotes.txt is empty) and False otherwise. 
* ```add_quote()``` - Requests quote information from user and adds it to the text file.
* ```tweet_quote()``` - Tweets last quote stored in quotes.txt file.
* ```prepare_tweet(text)``` - Helper function that creates appropriate hashtags from the book title and author's name.
