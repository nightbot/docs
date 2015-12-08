/*
Title: Rainwave
*/

Rainwave is a gaming radio network that plays raw game soundtracks, remixes, and more. You can utilize the Rainwave variable to list the now playing song on any of the Rainwave stations.

### Normal Usage

> $(rainwave `station`)

`station` is the station being looked up on Rainwave. It can be any of the following:

* `all` - All
* `game` - Game
* `chiptune` - Chiptune
* `ocremix` - OC Remix
* `covers` - Covers

#### Example for Normal Usage

> $(rainwave game)

would result in

> Battlefield - Those That Slay and Fall by Yuzo Koshiro

### Advanced Usage

> $(rainwave `station` "`formatted string`")

`station` is the station being looked up on Rainwave. It can be any of the following:

* `all` - All
* `game` - Game
* `chiptune` - Chiptune
* `ocremix` - OC Remix
* `covers` - Covers

`formatted string` is a string with the following mustache-tagged parameters:

* artist - The artist of the most recent scrobbled track
* title - The title of the most recent scrobbled track
* url - A link to the most recent scrobbled track on Last.fm

#### Example Usage

> $(rainwave ocremix "{{title}} by {{artist}} - {{url}}")

would result in

> The Vision of the Wind Fish by Sound Test - http://threshold.ocremix.org

## Examples

#### Adding a command to show chatters what song you're listening to on stream (if you're playing a station on Rainwave)

> !commands add !song $(rainwave `station`)