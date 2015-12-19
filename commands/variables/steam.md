/*
Title: Steam
*/

You can use the Steam variable to display various information about a specific Steam profile.

### Normal Usage

> $(steam `username`)

`username` is the Steam community ID being looked up

#### Example for Normal Usage

> $(steam night)

would result in

> Night is Offline since Sun Dec 06 2015 04:09:04 GMT-0500 (EST) - http://steamcommunity.com/id/night/

### Advanced Usage

> $(steam `username` "`formatted string`")

`username` is the Steam community ID being looked up

`formatted string` is a string with the following mustache-tagged parameters:

* *name* - Currently set player name
* *realName* - User's real name (if one is set)
* *profileUrl* - Link to the user's Steam community page
* *lastOnline* - The last time a user was online on Steam
* *status* - The current status of the user (Online, Offline, Busy, Away, Snooze, Looking to play, Looking to trade)
* *country* - The country the user resides in (if one is set)
* *gameId* - The game ID of a Steam game being played (if one is being played)
* *gameName* - The game being played (if one is being played)
* *gameUrl* - The link to the game's Steam page (if a game is being played)
* *gameServer* - The IP and port of the server being played on (if an eligible game is being played)

#### Example Usage

> $(steam night "{{name}} resides in {{country}} - {{profileUrl}}")

would result in

> Night resides in US - http://steamcommunity.com/id/night/

## Examples

#### Adding a command to show chatters your Steam profile info

> !commands add !steam $(steam `username`)

#### Adding a command to allow users in chat to lookup their own Steam profile

> !commands add !steamlookup $(steam $(query))