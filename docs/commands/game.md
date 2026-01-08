---
title: "!game"
sidebar_position: 5
---

The !game command displays the current game being played on the stream and allows you and your moderators to modify it.

## Usage

> !game `game name`

`game name` is the name of the game that you wish to change to. Only place a game name to change the current game. Omitting this value displays the current game.

### Examples

> !game

will return "night is playing League of Legends"

> !game League of Legends

will return "The stream game has been updated to: League of Legends"

**Note:** The default userlevel for the !game command is set to `everyone`. This implies that everyone can check the current game being streamed to the channel. Only moderators and higher userlevels can modify the game.