/*
Title: Provider
*/

The Provider variable can be used to show the service where Nightbot is receiving a command. It's useful when used as an argument for a UrlFetch.

## Usage

> $(provider)

would result depending on what service the command was used.

#### Provider Values

* `twitch` - When used in Twitch chat
* `youtube` - When used in YouTube Gaming
* `discord` - When used in a Discord message
* `mixer` - When used in Mixer chat