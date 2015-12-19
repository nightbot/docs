/*
Title: Lastfm
*/

You can use the Lastfm variable to display the most recent song scrobbled to a Last.fm account. This is useful when you use a scrobbling tool or enable scrobbling to Last.fm in Spotify and want viewers to know what track is playing on your stream.

### Normal Usage

> $(lastfm `username`)

`username` is the username being looked up on Last.fm

#### Example for Normal Usage

> $(lastfm night)

would result in

> The Reason by Hoobastank

### Advanced Usage

> $(lastfm `username` "`formatted string`")

`username` is the username being looked up on Last.fm

`formatted string` is a string with the following mustache-tagged parameters:

* *artist* - The artist of the most recent scrobbled track
* *title* - The title of the most recent scrobbled track
* *url* - A link to the most recent scrobbled track on Last.fm

#### Example Usage

> $(lastfm night "{{title}} by {{artist}} - {{url}}")

would result in

> The Reason by Hoobastank - http://www.last.fm/music/Hoobastank/_/The+Reason

## Last.fm + Spotify

A lot of streamers use Spotify for music on stream. If this is the case for you, you may want to connect your Spotify to Last.fm. You can do this in the Spotify settings:

1. Open Spotify settings
2. Scroll to Last.fm section
3. Click the "Connect to Last.fm" button to connect your Last.fm account to Spotify
4. Add a Nightbot command to show the most recent scrobbled song (shown under Examples below)

## Examples

#### Adding a command to show chatters what song you're listening to on stream (if you're scrobbling songs to Last.fm)

> !commands add !song $(lastfm `username`)