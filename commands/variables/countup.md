/*
Title: Countup
*/

You can utilize the countup variable to create commands that display a countup. For example, maybe you want to countup from a special event that happened on your stream.

## Usage

The countup variable accepts two kinds of arguments: a specific date/time or a specific time.

### Specific Date/Time

> $(countup `date/time`)

`date/time` is the specific date/time you wish to count up to

It can accept variants of dates, but it works best with dates in the format: `Month Day Year HH/MM/SS AM/PM TZ`

#### Example Usage

> $(countup Dec 25 2015 12:00:00 AM EST)

will result with a response in this format

> 1 day, 3 hours, 20 minutes, 30 seconds

### Specific Time

> $(countup `time`)

`time` is the specific time you wish to count up to (the countdown resets daily)

It can accept variants of dates, but you will find it works best with dates in the format: `HH/MM/SS AM/PM TZ`

#### Example Usage

> $(countup 5:00:00 PM EST)

will result with a response in this format

> 3 hours, 20 minutes, 30 seconds

## Examples

#### Adding a command to show chatters how long it's been since Christmas

> !commands add !christmas It has been days since Christmas $(countup Dec 25 2014 12:00:00 AM EST)
