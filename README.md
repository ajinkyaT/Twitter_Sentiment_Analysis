# Twitter Sentiment Analysis using Tweepy and TextBlob.
Twitter Sentiment Analysis using Python
Installation:

## Tweepy: tweepy is the python client for the official Twitter API.
Install it using following pip command:
```python
pip install tweepy
```
## TextBlob: textblob is the python library for processing textual data.
Install it using following pip command:
```python
pip install textblob
```
Also, we need to install some NLTK corpora using following command:
```python
python -m textblob.download_corpora
```
## Authentication:
In order to fetch tweets through Twitter API, one needs to register an App through their twitter account. Follow these steps for the same.

  Open this [link](https://apps.twitter.com/) and click the button: ‘Create New App’.
  Fill the application details. You can leave the callback url field empty.
  Once the app is created, you will be redirected to the app page.
  Open the ‘Keys and Access Tokens’ tab.
  Copy ‘Consumer Key’, ‘Consumer Secret’, ‘Access token’ and ‘Access Token Secret’.
  And paste it in sentiment.py file in relevant fields, as shown below.

```python
 def __init__(self):
        '''
        Class constructor or initialization method.
        '''
        # keys and tokens from the Twitter Dev Console
        consumer_key = 'XXXXXXXXXXXXXXXXXXXXXXXX'
        consumer_secret = 'XXXXXXXXXXXXXXXXXXXXXXXXXXXX'
        access_token = 'XXXXXXXXXXXXXXXXXXXXXXXXXXXX'
        access_token_secret = 'XXXXXXXXXXXXXXXXXXXXXXXXX'

```
## Code Implementation
open [sentiment.py](../master/sentiment.py)
## Here is how a sample output looks like when above program is run:

```python
Positive tweets percentage: 22 %
Negative tweets percentage: 15 %


Positive tweets:
RT @JohnGGalt: Amazing—after years of attacking Donald Trump the media managed
to turn #InaugurationDay into all about themselves.
#MakeAme…
RT @vooda1: CNN Declines to Air White House Press Conference Live YES! 
THANK YOU @CNN FOR NOT LEGITIMI…
RT @Muheeb_Shawwa: Donald J. Trump's speech sounded eerily familiar...
POTUS plans new deal for UK as Theresa May to be first foreign leader to meet new 
president since inauguration 
.@realdonaldtrump #Syria #Mexico #Russia & now #Afghanistan. 
Another #DearDonaldTrump Letter worth a read @AJEnglish 


Negative tweets:
RT @Slate: Donald Trump’s administration: “Government by the worst men.” 
RT @RVAwonk: Trump, Sean Spicer, et al. lie for a reason. 
Their lies are not just lies. Their lies are authoritarian propaganda.  
RT @KomptonMusic: Me: I hate corn 
Donald Trump: I hate corn too
Me: https://t.co/GPgy8R8HB5
It's ridiculous that people are more annoyed at this than Donald Trump's sexism.
RT @tony_broach: Chris Wallace on Fox news right now talking crap 
about Donald Trump news conference it seems he can't face the truth eithe…
RT @fravel: With False Claims, Donald Trump Attacks Media on Crowd Turnout 
Aziz Ansari Just Hit Donald Trump Hard In An Epic Saturday NIght Live Monologue
```

