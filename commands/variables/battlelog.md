/*
Title: Battlelog
*/

You can use the Battlelog variable to create commands that display user stats or status information from [EA's Battlelog](http://battlelog.battlefield.com/). This is useful for sharing the URL of the current Battlefield server you're playing in as well as letting your viewers see your player stats in-game.

## Usage

The Battlelog variable has two actions that you can perform: stats and status.

### Stats

> $(battlelog stats `platform` `game` `username`)

`platform` is the platform the stats are being looked up for (values can be `pc`, `ps3`, `ps4`, `xbox360`, and `xboxone`)

`game` is the game the stats are being looked up for (values can be `bf3`, `bf4`, `bfh`, and `mohw`)

`username` is the username being looked up on the specied platform

#### Example Usage

> $(battlelog stats pc bf4 iblindfolded)

would result in

> [Battlefield 4 stats on PC for iBlindfolded] Rank: Brigadier General VIII, Skill: 254, K/D: 3.47, W/L: 1.52, Kills: 15893, Score: 16,338,379, SPM: 1028.28, Accuracy: 12.00, Time Played: 11 days, 49 minutes, 0 seconds - More info at http://bf4stats.com/pc/iBlindfolded

### Status

> $(battlelog status <code>username</code>)

`username` is the EA account name on Battlelog being looked up

#### Example Usage

> $(battlelog status iblindfolded)

would result in

> iBlindfolded is currently online playing Battlefield 4 (PC) on =rTr= #1 ~ HARDCORE CONQUEST - More info at http://bit.ly/1Qa0y24

## Examples

#### Adding a command to show chatters what server you're playing on

> !commands add !battlelogstatus $(battlelog status `username`)

#### Adding a command to allow users in chat to lookup their own stats

> !commands add !battlelogstats $(battlelog stats $(query))
