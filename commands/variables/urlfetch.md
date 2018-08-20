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

Nightbot sends request headers that contain pertinent information of the user calling the command, the channel the command was called, and a response URL to POST a response.

### Headers

`Nightbot-Response-Url` - A response link where responses can be sent with a POST request without prior authorization. See [/channel/send](https://api-docs.nightbot.tv/#send-channel-message) in the API docs.

`Nightbot-User` - User data of the user who used the command that triggered the urlfetch. **Note:** This header is **not** sent when the urlfetch is called from a timer.

`Nightbot-Channel` - Channel data of the channel where the command was used.

#### Example Headers

> Nightbot-Response-Url: https://api.nightbot.tv/1/channel/send/TVRRM05UazRNVGsyT1RnNE1TOWthWE5...

> Nightbot-User: name=night&displayName=night&provider=twitch&providerId=11785491&userLevel=owner

> Nightbot-Channel: name=night&displayName=Night&provider=twitch&providerId=11785491

### JSON 

This variant of urlfetch will allow the api to be greater than 400 characters, however the response must be type JSON. This is most useful when paired with [eval](https://docs.nightbot.tv/commands/variables/eval) to get more dynamic results.

### Usage

> $(urlfetch json `url`)

`url` is a URL that returns a body of JSON

### Example Usage

#### Get Wikipedia Article from Query

> !commands add !wiki Wikipedia Article: $(eval const api = $(urlfetch json https://en.wikipedia.org/w/api.php?format=json&action=opensearch&search=$(querystring)); api.error || !api[1][0] ? 'Please add a query to the search' : `${api[1][0]} - ${api[3][0]}`)
