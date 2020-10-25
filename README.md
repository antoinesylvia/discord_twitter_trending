# discord_twitter_trending

Purpose: <br/>
Creates a discord bot that posts a list trending hashtags from the twitter api for a specified location automatically to a discord channel. <br/>

Requirements for auth config file:
<br/>
DISCORD_TOKEN: https://discord.com/developers/applications, create an app the on left side you will see "bot". Click bot and reveal the token, post inside config.
<br/>
TWITTER_API_KEY: https://developer.twitter.com 
<br/>
TWITTER_API_SECRET_KEY: https://developer.twitter.com
<br/>
TWITTER_ACCESS_TOKEN: https://developer.twitter.com
<br/>
TWITTER_ACCESS_TOKEN_SECRET: https://developer.twitter.com

Install the following libraries:
pip3 install tweepy
pip3 install discord.py

Examples: <br/>
```tb clear 5``` - Removes last 5 messages from discord channel. <br/>
```tb clear 10``` - Removes last 10 messages from discord channel. <br/>
```tb help``` - Posts help menu to discord channel. <br/>
```tb trend united states 60``` - Post trending hashtags in the US to a discord channel every minute. <br/>
```tb trending fortaleza 10``` - Post trending hashtags in Fortaleza, Brazil to a discord channel every 10 seconds. <br/>
```tb trend barcelona_es 3600``` - Post trending hashtags in Barcelona, Spain to a discord channel every hour. <br/>
```tb stop``` - Stops bot from posting automatically to discord channel. <br/>

If you want to run this bot as a Windows service. Simply download NSSM and stick it in any folder already mentioned in the system account environment variables like Windows or System32. Next step is to open a command prompt and type the following:
NSSM Install (Name of the Service, whatever you want to call it)

A GUI should pop up:
For Path - Do a direct mapping to your Python3 executable.
For Startup Directory - Just pick the folder where your main.py file is located.
For Arguments - Just type without quotes "main.py".
Hit the edit/install button once done.

Your bot should now be online with Discord, if you Windows Service is running for this app:
Start -> Run -> services.msc --> Look for name of app and ensure it's running. 
