/*
Title: General Setup
Sort: 5
*/

## General Setup Guide for Nightbot

This page's purpose is a general guide for new users who want to use Nightbot. This guide will review some of the basics of using Nightbot with more advanced usage on the individual doc site pages. Nightbot is currently available for Twitch, YouTube, Trovo, Noice, and SOOP!

### Sign in & Dashboard

To begin head to the [Nightbot Homepage](https://nightbot.tv/) and sign in using the service you intend to use Nightbot with. Upon granting access you are directed to the Nightbot Control Panel.

The Control Panel is the central hub to controlling Nightbot. The Dashboard also displays stats such as chat activity, command usage, and spam filters. Using the navigation bar on the left you can edit a specific area of Nightbot.

### Make Nightbot Join Your Channel

On the Dashboard, click the Join Button on the top-right of the page to have Nightbot join your channel. You will then have a popout with instructions for making Nightbot a moderator in your channel.

**For YouTube:** Nightbot for YouTube will only join your channel when you are live and your stream is public. This is currently due to rate limits on YouTube's API.

### Custom Commands

After adding Nightbot, you can now begin with creating custom commands. Custom commands are an important part of any stream, making information easier to access. Commands are managed in the [Custom Command](https://nightbot.tv/commands/custom) page in the  Control Panel.

When adding a command you will need a command name (usually leading with an exclamation mark) and a command response. [Custom Variables](https://docs.nightbot.tv/commands/variableslist) can customize your commands with features like Click-To-Tweet links or displaying the weather of a location.

Commands can also be managed using the [!commands](https://docs.nightbot.tv/commands/commands) command.

### Timers

The [Timers](https://nightbot.tv/timers) page contains configurable timers where Nightbot displays a message every so often. The time interval and chat lines required can be changed to your liking and can be enabled and disabled as needed.

### Regulars

Regulars are users who are more privileged than normal users. You may want regulars to be ignored when dealing with Spam Filters or you might want them to have access to certain commands.

The solution is for you to add users as Regulars into Nightbot. Users can be managed in the [Regulars](https://nightbot.tv/regulars) page, just click the Add User button and enter the Username. Those users are now defined as a regular of the channel and you can filter separate user-specific commands around them.

This can also be done by using the [!regulars command](https://docs.nightbot.tv/commands/regulars).

### Song Request

Song Request is the ability for music in your stream to go into viewers hands.

A personal playlist is provided as a backup song list if the queue happens to run out of requests. Alternatively, Monstercat songs can also be used rather than your personal playlist.

For more information about Song Request see the [AutoDJ](https://nightbot.tv/song_requests) page and [AutoDJ Guide](https://docs.nightbot.tv/control-panel/autodj).

### Spam Filters

Spam Filters within Nightbot can help deal with users who spam. Offering filters including Capitalization, Links, Symbols,  and Custom Blacklist. All filters can be edited in the [Spam Protection](https://nightbot.tv/spam_protection) page within the Nightbot Control Panel or with the [!filters](https://docs.nightbot.tv/commands/filters) command.

---

More in-depth information about the topics here can be found throughout the Nightbot Documentation. Reach out to us on the [forums](https://community.nightdev.com/c/nightbot) for any questions.
