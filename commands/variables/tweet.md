/*
Title: Tweet
*/

The tweet variable creates a click-to-tweet link. This is useful for providing chatters with a link to tweet out your stream.

## Usage

> $(tweet `message`)

`message` is the message to be tweeted

#### Example Usage

> $(tweet Come check out Night's Twitch stream: http://twitch.tv/night)

would result in

> http://bit.ly/someshortenedlink

## Examples

#### Adding a command to let viewers tweet out your stream

> !commands add !tweet $(tweet Come watch @`TwitterUser` while they play $(twitch $(channel) "{{game}} on Twitch! {{url}}"))