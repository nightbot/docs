/*
Title: XBL
*/

You can use the XBL variable to create commands that display information about a specific Xbox Live profile.

## Usage

> $(xbl `gamertag`)

`gamertag` is the Xbox Live gamertag being looked up

#### Example Usage

> $(xbl night)

would result in

> night has a gamerscore of 105056 and is currently online playing Call of Duty®: Black Ops III Playing Multiplayer on Call of Duty®: Black Ops III.

## Examples

#### Adding a command to show chatters your gamertag stats

> !commands add !xbl $(xbl `gamertag`)

#### Adding a command to allow users in chat to lookup their own gamertag

> !commands add !xbllookup $(xbl $(query))