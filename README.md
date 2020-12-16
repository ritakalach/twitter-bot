# Twitter Bot 🐦🤖 
I wanted to share some book quotes (which are stored in a text file) on Twitter, but didn't want to manually copy and paste each one. Naturally, I decided to automate this task using Twitter's API and Python's *tweepy* library. I also used *re* library to create hashtags based on the book's title and author's name.

## Running the code
Download [*tweet_quote.py*](code/tweet_quote.py) and [*quotes.txt*](data/quotes.txt) files to the same directory. In *tweet_quotes.py* make sure to update lines 136-139 with you account credentials. Open your terminal and run ```python3 tweet_quote.py```. You'll be prompted for input. Type "tweet" in your terminal to tweet the last quote stored in *quotes.txt*. You can also type "shuffle quotes", "add quote", or "exit".

If you wish to add your own quote, it must be in the following format: "Quote text.",Book Title,Book Author

## Available functions
* ```request_user_input()``` - Type one of the following in the command line: tweet, shuffle quotes, add quote, or exit.
* ```shuffle_quotes()``` - Shuffles quotes currently stored in text file. (I sometimes do this after adding a lot of new quotes from the same book.)
* ```is_file_empty(lines)``` - Takes lines as input; returns True if there are no lines (meaning quotes.txt is empty) and False otherwise. 
* ```add_quote()``` - Requests quote information from user and adds it to the text file.
* ```tweet_quote()``` - Tweets last quote stored in quotes.txt file.
* ```prepare_tweet(text)``` - Helper function that creates appropriate hashtags from the book title and author's name.
