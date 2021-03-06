# ChessBot
A chess bot for Discord, made with discord.py and python-chess.

![Screenshot of the bot](https://user-images.githubusercontent.com/4065977/66155614-bb7b2180-e628-11e9-9e5a-0fb3c15bdc5c.png)

## Setup
1. Create a file called `env_variables.sh` that looks like this:
```
#!bin/bash

export TOKEN="YOUR DISCORD BOT TOKEN"
export DB_PATH="PATH TO YOUR DATABASE"

```
2.
```
pip3 install -r requirements.txt
```

## Running the bot
```
source env_variables.sh
python3 -m chessbot
```

## Available commands
`/help` - Displays the help message.  
`/play @someone` - Starts a game with @someone.  
`/move (SAN move) [Game ID]` - Moves a piece according to the standard algebraic notation in the game.  
`/status [Game ID]` - Displays the current status of the game.  
`/offer (Action) [Game ID]` - Offers an action in the game. Possible actions: *draw*, *undo*.  
`/accept [Game ID]` - Accepts an action in the game.  
`/concede [Game ID]` - Concedes in the game.  
`/games [all]` - Shows your games.  
`/elo` - Shows your elo rating.  
`/leaderboard [Top N]` - Shows the global leaderboard (3 ≤ N ≤ 50).  
