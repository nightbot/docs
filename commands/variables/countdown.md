/*
Title: Countdown
*/

You can utilize the countdown variable to create commands that display a countdown. For example, maybe you want to countdown until a special occasion stream or maybe you stream daily starting at a specific time. This will work great for both of those use-cases.

## Usage

The countdown variable accepts two kinds of arguments: a specific date/time or a specific time.

### Specific Date/Time

> $(countdown `date/time`)

`date/time` is the specific date/time you wish to count down to. It can accept variants of dates, but you will find it works best with dates in the format: Month Day Year HH/MM/SS AM/PM TZ

#### Example Usage

> $(countdown Dec 25 2015 12:00:00 AM EST)

will result with a response in this format

> 1 day, 3 hours, 20 minutes, 30 seconds

### Specific Time

> $(countdown `time`)

`time` is the specific time you wish to count down to. The countdown resets daily. It can accept variants of dates, but you will find it works best with dates in the format: HH/MM/SS AM/PM TZ

#### Example Usage

> $(countdown 5:00:00 PM EST)

will result with a response in this format

> 3 hours, 20 minutes, 30 seconds

## Examples

#### Adding a command to show chatters when your stream starts daily

> !commands add !starting The stream is starting in $(countdown 5:00:00 PM EST)

#### Adding a command to show chatters when your special Christmas stream begins

> !commands add !christmas Christmas Countdown: $(countdown Dec 25 2015 12:00:00 AM EST)
