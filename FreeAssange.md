---
layout: home
title: FreeAssange
comments: true
---

 * This tutorial explains how to create a python script to follow hashtags on twitter. Our biggest motivation is to give some support. Forgive me for my googled english, i am brazilian.

### Initially have python and pip installed on your linux distro:

Something like:
python --version
Python 2.7.12
python3 --version
Python 3.5.2
pip --version
pip 18.0
pip3 --version
pip 8.1.1
That's enough.

### Install too:

 * python-setuptools

`sudo apt-get install python-setuptools`

 * pip (easy_install pip)

`sudo easy_install pip`

 * twython

`sudo pip install twython`

### Create an app on twitter

 * Create an [app on twitter](https://developer.twitter.com/en/docs/basics/authentication/guides/access-tokens.html) and copy the credentials (consumer_key, consumer_secret, access_token, access_secret)

### Create two files like this (on the same diretory):

auth.py
```py
consumer_key        = 'your_consumer_key'
consumer_secret     = 'your_consumer_secret'
access_token        = 'your_access_token'
access_token_secret = 'your_access_token_secret'
```
trackerFreeAssange.py
```py
#!/usr/bin/env python
from twython import TwythonStreamer
from auth import (
    consumer_key,
    consumer_secret,
    access_token,
    access_token_secret
)
class MyStreamer(TwythonStreamer):
    def on_success(self, data):
        if 'text' in data:
            print(data['text'])
stream = MyStreamer(
    consumer_key,
    consumer_secret,
    access_token,
    access_token_secret
)
stream.statuses.filter(track='#FreeAssange')
```
### Run trackerFreeAssange!

Run `python trackerFreeAssange.py` run the script on the terminal to keep track of all hashtag occurrences in real time.

#FreeAssange

<p align="center">
  <img width="460" height="300" src="/assets/FreeAssange.png">
</p>