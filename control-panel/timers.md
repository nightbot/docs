/*
Title: Timers
Sort: 3
*/

Nightbot Timers have the ability to send messages on specific intervals. They are frequently used for social media links an general chat notifications.

## Usage

Timers can be created and managed on the [Timers](https://beta.nightbot.tv/timers) page in the control panel.

### Creating a Timer

Creating a Timer for your chat couldn't be any easier.

First head over to the [Timers](https://beta.nightbot.tv/timers) page.

In the top right corner of the panel, click the blue Add button which will open up a popup allowing you to create a timer.

#### Settings

- *Name* - This is your timer name. This has no real significance but to give you a quick reference to what your timer does. Ex. Twitter Message

- *Message* - What do you want your timer's message to say when it gets shown in the chat? You can use [Variables](https://docs.nightbot.tv/commands/variables) in your messages to make dynamic messages.

- *Interval* - Move the slider to the desired amount of time before the timer repeats. For example, 15 minute intervals will activate at 2:00, 2:15, 2:30, etc.

- *Chat Lines* - This is the minimum amount of chat lines required to activate the timer. This is useful in slow chats to prevent Nightbot from spamming in an empty channel.

**Note**: The timer will first wait the specified amount of time and then check to see if the specified number of chat lines have passed before displaying a message. This can account for timer messages not displaying after passing their interval.

### Managing Timers

On the Panel screen you will see a list of all timers you have created. All displaying their current status, timer name, timer message, and action buttons. 

#### Action Buttons

- *Disable/Enable* - The Disable/Enable button can be used to turn off and on your timers. This will change the far left column status after clicking.

- *Edit* - The Edit button will re-open the popup to edit current timers. Be sure to hit Submit to save changes otherwise changes will be lost.

- *Delete* - The Delete button will prompt you to confirm that you want to remove your timer.

### Tips

- **Less is More** - Keep your amount of timers and the length between timers showing reasonable. Chatters do not like being spammed.

- **Change them up** - Don't be afraid to change a timers message, either to new changes such as a Twitter post or a link to a shirt your trying to advertise, change the content frequently. And with [Variables](https://docs.nightbot.tv/commands/variables) you can set messages that update automatically.
