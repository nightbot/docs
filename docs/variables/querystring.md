---
title: "QueryString"
---

The querystring variable prints a url-encoded string of the user's text after a command. This is useful when combined with the urlfetch variable in cases where data is being passed to a server via querystring.

## Usage

> $(querystring)

The querystring also accepts arguments that will return a url-encoded string.

## Alternate Usage

> $(querystring $(twitch $(channel) "{'{{'}url{'}}'}}"))

will return

> https%3A%2F%2Fwww.twitch.tv%2Fnight