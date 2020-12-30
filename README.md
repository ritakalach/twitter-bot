# Twitter Bot 🐦🤖 
I had a backlog of book quotes stored in a text file that I wanted to share on Twitter, but I didn't want to manually copy and paste each one. Naturally, I decided to automate this task via the Twitter API. I used Python's *Tweepy* library to accomplish this.


## Functions
* ```request_user_input()``` - type one of the following in the command line: "tweet", "shuffle quotes", "add quote", or "exit"
* ```shuffle_quotes()``` - shuffles quotes currently stored in text file (I sometimes do this after adding a lot of new quotes from the same book)
* ```is_file_empty(lines)``` - takes lines as input and returns True if there are no lines (meaning quotes.txt is empty) and False otherwise
* ```add_quote()``` - requests quote information from user and adds it to the text file
* ```tweet_quote()``` - tweets last quote stored in quotes.txt file
* ```prepare_tweet(text)``` - helper function that creates appropriate hashtags from the book title and author's name


## Running the code
Download [*tweet_quote.py*](tweet_quote.py) and [*quotes.txt*](quotes.txt) files to the same directory. In *tweet_quotes.py* make sure to update lines 136-139 with your account credentials. Open the terminal and run ```python3 tweet_quote.py```. You'll be prompted for input. Type "tweet" in the terminal to tweet the last quote stored in *quotes.txt*. You can also type "shuffle quotes", "add quote", or "exit".

If you wish to add your own quote, it must be in the following format: "Quote text.",Book Title,Book Author


## Example
Say the last line in the text file was: "I hope your bacon burns.",Diana Wynne Jones,Howl's Moving Castle

Running the code would produce the following tweet:

<img src="tweet.jpg" width = 300> 
