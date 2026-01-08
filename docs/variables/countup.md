---
title: "Countup"
---

You can use the countup variable to create commands that display the time since a specified date. For example, maybe you want to countup from a special event that happened on your stream.

## Usage

The countup variable accepts two kinds of arguments: a **date/time** or a **time**

### Date/Time

> $(countup `date/time`)

`date/time` is the specific date/time you wish to count up to

It can accept variants of dates, but you will find it works best with dates in the format: `MM DD YYYY HH:MM:SS AM/PM TZ`, `MM` is the month, `DD` is the day, `YYYY` is the year, `HH` is the hour, `MM` is the minutes, `SS` is the seconds, `AM/PM` is `AM` *or* `PM`, and `TZ` is the timezone. For a list of supported timezones, check out [the time variable page](https://docs.nightbot.tv/variables/time#timezones).

#### Example Usage

> $(countup Dec 25 2015 12:00:00 AM EST)

will result with a response in this format

> 1 day 3 hours 20 minutes 30 seconds

### Time

> $(countup `time`)

`time` is the specific time you wish to count up to (the countup resets daily)

It can accept variants of times, but you will find it works best with times in the format: `HH:MM:SS AM/PM TZ`, where `HH` is the hour, `MM` is the minutes, `SS` is the seconds, `AM/PM` is `AM` *or* `PM`, and `TZ` is the timezone. For a list of supported timezones, check out [the time variable page](https://docs.nightbot.tv/variables/time#timezones).

#### Example Usage

> $(countup 5:00:00 PM EST)

will result with a response in this format

> 3 hours 20 minutes 30 seconds

## Examples

#### Adding a command to show chatters how long it's been since Christmas

> !commands add !christmas It has been days since Christmas $(countup Dec 25 2014 12:00:00 AM EST)
