/*
Title: Twitch
*/

You can utilize the Twitch variable to list profile information for Twitch accounts.

### Normal Usage

> $(twitch `username`)

`username` is the Twitch user being looked up.

#### Example for Normal Usage

> $(twitch goldglove)

would result in

> GoldGlove is currently live playing Super Mega Baseball at 720p, 60 fps with 7,780 viewers since Mon Dec 07 2015 22:10:56 GMT-0500 (EST) (4 hours, 3 minutes, 50 seconds) - http://www.twitch.tv/goldglove

### Advanced Usage

> $(twitch `username` "`formatted string`")

`username` is the Twitch user being looked up.

`formatted string` is a string with the following mustache-tagged parameters:

* *name* - username
* *displayName* - display name
* *url* - channel page link
* *status* - offline, live, or playing a playlist
* *title* - stream title
* *game* - stream game
* *createdAt* - date/time user account was created
* *createdLength* - length of time user has been created (years, months, days, hours, minutes, seconds)
* *viewers* - current number of viewers
* *views* - current number of views
* *followers* - current number of followers
* *resolution* - stream resolution (if live)
* *fps* - stream fps (if live)
* *uptimeAt* - date/time user went live (or started playing a playlist)
* *uptimeLength* - length of time user has been live (or started playing a playlist) (years, months, days, hours, minutes, seconds)

#### Example Usage

> $(twitch goldglove "{{displayName}} has {{followers}} followers")

would result in

> GoldGlove has 1,037,856 followers

## Examples

#### Adding a command to show chatters your channel's uptime

> !commands add !uptime Stream uptime: $(twitch $(channel) "{{uptimeLength}}")

#### Adding a command to show chatters your channel's stats

> !commands add !stats Channel stats: $(twitch $(channel) "{{viewers}} viewers, {{views}} views, {{followers}} followers")