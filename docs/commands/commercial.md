---
title: "!commercial"
sidebar_position: 12
---

The !commercial command will run a commercial for a specified length. This command will only work if your channel is partnered. 

## Usage

> !commercial `duration` `[silent]`

`duration` is the length you want the commercial to run for. The duration can be `30`, `60`, `90`, `120`, `150` or `180` seconds.

`[silent]` is an optional value that will hide the Nightbot response, particularly for use in Timers.

### Examples

> !commercial 30

will start a commercial with a duration of 30 seconds. 

> !commercial 60 silent

will start a commercial with the Nightbot response hidden.

**Note:** The default UserLevel for the !commercial command is set to `owner`. 
