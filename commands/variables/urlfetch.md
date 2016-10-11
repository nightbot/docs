/*
Title: UrlFetch
*/

The urlfetch (formerly customapi) variable calls a remote url to retrieve and display a response. It's useful for building more complex commands that Nightbot does not support.

## Usage

> $(urlfetch `url`)

`url` is a URL that returns a body in *plain text* with less than 400 characters in its response

### Examples

Check out the Custom APIs sub-forum on our Community Forum: https://community.nightdev.com/c/nightbot/custom-apis

## Advanced Usage

Nightbot sends request headers that contain pertinent information of the user calling the command, the channel the command was called and and a response URL to POST a response.

### Headers

`Nightbot-Response-Url` - A response link where responses can be send with a POST request without prior authorization. See [/channel/send](https://api-docs.nightbot.tv/#send-channel-message) in the API docs.

`Nightbot-User` - User data of the user who used the command that triggered the urlfetch. **Note:** This header is **not** sent when the urlfetch is called from a timer.

`Nightbot-Channel` - Channel data of the channel where the command was used.

### Example Headers

`Nightbot-Response-Url: https://api.nightbot.tv/1/channel/send/TVRRM05UazRNVGsyT1RnNE1TOWthWE5qYjNKa0x6VTJOekl5TkdabE9URXhOV0V6T0dZMU1URTBZV013WlM4eE16a3lNelkxTkRjMk1UTTFOVFkzTXpZdk1UTTVNak0yTnpBME9UUTFPVFl6TURBNDo5ZmFlNjM5ODI4NmFkMmM0NDk1ZjkxYjk2MTQyMWI5ZDI0Y2EwYjRlZDA3NTIzNTE1MjU4ZWIzZDI0ZGEwNTRl`

`Nightbot-User: name=night&displayName=night&provider=twitch&providerId=11785491&userLevel=owner`

`Nightbot-Channel: name=night&displayName=Night&provider=twitch&providerId=11785491`