---
title: "Bluesky"
---

The Bluesky variable creates a click-to-post link for Bluesky. This is useful for providing chatters with a link to post about your stream. The generated link is automatically shortened.

## Usage

> $(bluesky `message`)

`message` is the message to be posted

#### Example Usage

> $(bluesky Come check out Night's Twitch stream: http://twitch.tv/night)

would result in

> https://go.night.bot/someshortenedlink

## Examples

#### Adding a command to let viewers post about your stream

> !commands add !bluesky $(bluesky Come watch @`BlueskyUser` while they play $(twitch $(channel) "{'{{'}game{'}}'}} on Twitch! {'{{'}url{'}}'}}"))
