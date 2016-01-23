/*
Title: Nightbot App Beta
Sort: 2
*/

In order to provide some extra functionality to song requests, we've created a small app for Windows and OSX. With this app, you'll be able to show the current song in your streaming software (OBS/XSplit/etc.), use hotkeys for song requests, and use Spotify for song requests.

## Download

* [Windows v0.0.1-alpha](https://beta.nightbot.tv/dl/nightbot_v0.0.1_win.exe)
* [OSX v0.0.1-alpha](https://beta.nightbot.tv/dl/nightbot_v0.0.1_osx.zip)

## Current Song Output

On Windows and OSX, we output a file in the Nightbot folder within your Documents folder. Here are the default paths:

* Windows: `%USERPROFILE%\Documents\Nightbot\`
* OSX: `/Users/USERNAME/Documents/Nightbot/`

## Hotkeys

We have added global hotkeys to make controlling song requests when streaming easier. These hotkeys make use of media keys, so if your keyboard does not support them you're not able to use them at this time.

* Volume Up: `Ctrl/Cmd` + `Shift` + `U`
* Volume Down: `Ctrl/Cmd` + `Shift` + `D`
* Skip Song: `Fast Forward Media Key`
* Play/Pause Toggle: `Play/Pause Media Key`

## Spotify

To use Spotify, simply open Spotify **before** launching the Nightbot app and then head to the song requests player within the app. Then, open the song requests settings and enable Spotify under the "Providers" setting and optionally set Spotify as the "Search Provider" to let users search for music by name/artist through Spotify. Spotify must remain open in order for music to remain playing.

**Volume cannot be changed within the control panel for Spotify, only within Spotify's player.** This is a limitation that cannot be worked around, unfortunately.

### Copyright FYI

Be aware that streaming copyrighted music content may result in negative consequences for your stream. Many music content producers (Monstercat, Ninety9Lives, etc.) are starting to offer licensing for their content to be played on YouTube/Twitch. We recommend setting up a channel playlist full of licensed/free music and then restricting requested songs to the channel playlist (this can be configured in the song request settings). This ensures you control the library of music that can be played on your stream and prevents viewers from causing you to break any laws by streaming copyrighted content.

## Customizability

We are aware that users may want to customize the hotkeys and the output of the current song text file. This is an initial app release and these features do not exist yet. We'll be adding more features to this app over time.