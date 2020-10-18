/*
Title: Provider
*/

The Provider variable can be used to show the service where Nightbot is receiving a command. It's useful when used as an argument for a [UrlFetch](https://docs.nightbot.tv/commands/variables/urlfetch).

## Usage

> $(provider)

would result depending on what service the command was used.

#### Provider Values

* `twitch` - When used in Twitch chat
* `youtube` - When used in YouTube live chat
* `discord` - When used in a Discord message
