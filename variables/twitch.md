/*
Title: Twitch
*/

You can use the Twitch variable to display various profile information about a specific Twitch account.

### Normal Usage

> $(twitch `username`)

`username` is the Twitch user being looked up

#### Example for Normal Usage

> $(twitch night)

would result in

> Night is currently live playing Super Mario Kart at 720p, 60 fps with 64 viewers since Mon Dec 07 2015 22:10:56 GMT-0500 (EST) (4 hours, 3 minutes, 50 seconds) - http://www.twitch.tv/night

### Advanced Usage

> $(twitch `username` "`formatted string`")

`username` is the Twitch user being looked up

`formatted string` is a string with the following mustache-tagged parameters:

* *name* - username
* *displayName* - display name
* *url* - channel page link
* *status* - offline, live, or playing a playlist
* *title* - stream title
* *game* - stream game
* *tags* - stream tags
* *createdAt* - date/time user account was created
* *createdLength* - length of time user has been created (years, months, days, hours, minutes, seconds)
* *viewers* - current number of live viewers
* *views* - current number of channel views
* *followers* - current number of channel followers
* *resolution* - stream resolution (if live)
* *fps* - stream fps (if live)
* *uptimeAt* - date/time user went live (or started playing a playlist)
* *uptimeLength* - length of time user has been live (or started playing a playlist) (years, months, days, hours, minutes, seconds)
* *subscriberCount* - the number of subscribers a channel has (only available when querying from the desired channel)

#### Example Usage

> $(twitch night "{{displayName}} has {{followers}} followers")

would result in

> Night has 14,359 followers

## Examples

#### Adding a command to show chatters your channel's uptime

> !commands add !uptime Stream uptime: $(twitch $(channel) "{{uptimeLength}}")

#### Adding a command to show chatters your channel's stats

> !commands add !stats Channel stats: $(twitch $(channel) "{{viewers}} viewers, {{views}} views, {{followers}} followers")
