/*
Title: UserLevel
*/

The userlevel variable prints the userlevel of the user calling the command. It's useful when used within a UrlFetch variable.

## Usage

> $(userlevel)

#### Example Usage

> $(userlevel)

would result in

> owner

if the current chat was nightdev's and nightdev called the command

#### Available UserLevel Values

* owner - Channel Owner
* moderator - Channel Moderator
* regular - Nightbot Regular (users added to the regulars list within the control panel)
* subscriber - Paid Channel Subscriber
* everyone - Normal User
