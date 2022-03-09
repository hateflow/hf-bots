# HateFlow Social Media Bots

This repository contains bots that reply to hate speech. It is using the [HateFlow](https://hateflow.de) API documented [here](https://docs.hateflow.de).
## Installation
```bash
pip3 install -r requirements.txt
```
## Twitch
1. Create an account on Twitch.
2. Request an OAuth code and update the `.env` file accordingly.
3. Start bot in read mode: `python3 twitch.py`

If you want to reply to detected comments, uncomment the last line of `event_message` in `twitch.py`.


## Reddit
1. Create an account on Reddit.
2. Create a [Reddit application](https://ssl.reddit.com/prefs/apps/) and update the `.env` file accordingly.
3. Start the bot in read mode: `python3 reddit.py`

The default setting is the subreddit "me_irl". If you want to reply to detected comments, uncomment 
the last line of `process_comments` in `reddit.py`. You can customize the subreddit or post at the end of the file.