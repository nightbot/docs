---
title: "Channel"
---

The channel variable just prints the current channel. It's useful when used within nested variables.

## Usage

> $(channel)

#### Example Usage

> $(channel)

would result in

> nightdev

if the current chat was nightdev's

## Examples

#### Adding a command to show how many Twitch followers the current channel has

> !commands add !followers $(channel) has $(twitch $(channel) "{'{{'}followers{'}}'}} followers!")