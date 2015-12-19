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

#### UserLevel Values

* **owner** - Channel Owner
* **moderator** - Channel Moderator
* **regular** - Nightbot Regular (users in the [regulars](https://docs.nightbot.tv/control-panel/regulars) list)
* **subscriber** - Paid Channel Subscriber
* **everyone** - Normal User *(default)*