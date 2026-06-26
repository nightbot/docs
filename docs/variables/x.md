---
title: "X"
---

The X variable creates a click-to-post link for X (formerly Twitter). This is useful for providing chatters with a link to post about your stream. The generated link is automatically shortened.

> **Note:** `$(tweet)` is an alias for `$(x)` and works identically.

## Usage

> $(x `message`)

`message` is the message to be posted

#### Example Usage

> $(x Come check out Night's Twitch stream: http://twitch.tv/night)

would result in

> https://go.night.bot/someshortenedlink

## Examples

#### Adding a command to let viewers post about your stream

> !commands add !x $(x Come watch @`XUser` while they play $(twitch $(channel) "{'{{'}game{'}}'}} on Twitch! {'{{'}url{'}}'}}"))
