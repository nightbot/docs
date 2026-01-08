---
title: "Timers"
sidebar_position: 6
---

Nightbot Timers have the ability to send messages at specific intervals. Frequently used for social media links and general chat notifications.

## Usage

Timers can be created and managed on the [Timers](https://nightbot.tv/timers) page in the control panel.

### Creating a Timer

Creating a Timer for your chat couldn't be any easier.

First head over to the [Timers](https://nightbot.tv/timers) page.

In the top right corner of the panel, click the blue Add button which will open up a popup allowing you to create a timer.

#### Settings

- *Name* - This is your timer name. This has no real significance but to give you a quick reference to what your timer does. Ex. Twitter Message

- *Message* - What do you want your timer's message to say when it gets shown in the chat? [Custom Variables](https://docs.nightbot.tv/commands/variableslist) can also be used to make dynamic messages.

- *Interval* - Move the slider to the desired amount of time before the timer repeats. For example, 15 minute intervals will activate at 2:00, 2:15, 2:30, etc.

- *Chat Lines* - This is the minimum amount of chat lines (measured in lines per 5 minutes) required to activate the timer. This is useful in slow chats to prevent Nightbot from spamming in an empty channel.

- *Alias* - If you want this timer to call a command, specify that command here. Note that the input passed to the listed alias is the message field above, so to pass data to the command you need to place it in the message field. You can also use most variables in the message field.

**Note**: The timer will first wait the specified amount of time and then check to see if the specified number of chat lines have passed before displaying a message. This can account for timer messages not displaying after passing their interval.

### Managing Timers

The Panel screen lists all timers; displaying their current status, name, message, and action buttons.

#### Action Buttons

- *Disable/Enable* - Can be used to turn off and on your timers. This will change the far left column status after clicking.

- *Edit* - Reopen the popup to edit current timers. Be sure to hit Submit to save changes otherwise changes will be lost.

- *Delete* - The Delete button will open a prompt to remove that timer.

### Tips

- **Less is More** - Keep your amount of timers and the length between timers showing reasonable. Users do not like being spammed.

- **Change them up** - Don't be afraid to change a timers message, either to new changes such as a Twitter post or a link to a shirt your trying to advertise, change the content frequently. And with [Variables](https://docs.nightbot.tv/commands/variableslist) you can set messages that update automatically.
