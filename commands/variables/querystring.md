/*
Title: QueryString
*/

The querystring variable prints anything a user types after a command, but in url-encoding. This is useful when combined with the urlfetch variable in cases where data is being passed to a server via querystring.

## Usage

> $(querystring)

The querystring also accepts arguments that will return a url-encoded string.

## Alternate Useage

> $(querystring $(twitch $(channel) "{{url}}"))

will return

> https%3A%2F%2Fwww.twitch.tv%2Fnight