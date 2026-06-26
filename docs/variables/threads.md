---
title: "Threads"
---

The Threads variable creates a click-to-post link for Threads. This is useful for providing chatters with a link to post about your stream. The generated link is automatically shortened.

## Usage

> $(threads `message`)

`message` is the message to be posted

#### Example Usage

> $(threads Come check out Night's Twitch stream: http://twitch.tv/night)

would result in

> https://go.night.bot/someshortenedlink

## Examples

#### Adding a command to let viewers post about your stream

> !commands add !threads $(threads Come watch @`ThreadsUser` while they play $(twitch $(channel) "{'{{'}game{'}}'}} on Twitch! {'{{'}url{'}}'}}"))
