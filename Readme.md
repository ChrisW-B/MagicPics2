#Twitter Magic Gifs Bot

Just a simple Tweepy based bot that replies to people it follows with relevant gifs from Giphy

"Inspired" by boredom and the old @MagicPixx bot

Make sure to install Tweepy, TextBlob, Wordfilter and my updated version of Giphypop before running!
You also need to set up textblob before this can run
```sh
pip install tweepy textblob wordfilter requests git+git://github.com/ChrisW-B/giphypop 
python -m textblob.download_corpora
```

After that, its as simple as setting up a config.py file like so, where badwords are words the bot will not search for
```python
consumer_key = "XXXXXXXX"
consumer_secret = "XXXXXXXX"
access_token = "XXXXXXXX-XXXXXXXX"
access_token_secret = "XXXXXXXX"
badwords = [
    'XXX',
    'XXXXX']
```

and then running `python magicgif.py`


Things I might try to add
- Improving NLP to search for key phrases instead of just nouns/verbs
