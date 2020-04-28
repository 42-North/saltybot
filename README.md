# Salty Bot
An auto-betting Chrome Extension bot for [saltybet](https://www.saltybet.com/).

## Prerequisites
a) Python 2.7
1. Download from https://www.python.org/download/releases/2.7/
2. Install with everything set to default

b) Flask
1. Open a command prompt at C:\Python27
2. Run the command "pip install flask" to install Flask

## Installation
1. Open Chrome://extensions
2. Toggle on Developer Mode
3. Drag the extension folder onto the extension page

## Starting the Bot
1) Open a command prompt at C:\<install path>\saltybot-master\server
2) Run the command "python server.py"
3) Now navigate to [saltybet](https://www.saltybet.com/) and watch as you ascend to salt royalty (you're going to have to give the bot some time to collect data though). 

## Current Betting Strategy

SaltyBot currently assigns an elo rating to each player using [this](http://en.wikipedia.org/wiki/Elo_rating_system#Performance_rating) method and picks wagers based on elo difference.

If there is no collected data for either player, SaltyBot will just bet a $1 on player 1 in case an upset occurs.

## Am I Really Winning Money?

SaltyBot records its stats.  Check out `server/meta.json` or just navigate to [127.0.0.1:5000/stats](http://127.0.0.1:5000/stats) to see how your bot is doing. 
(This may not be working)


