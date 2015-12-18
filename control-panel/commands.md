/*
Title: Commands
Sort: 1
*/

The crux of any chat bot is its commands. Commands allow people to perform bot actions within chat. There are built-in default commands, and Nightbot also offers the ability to create your own custom commands.

## Default Commands

The majority of the default commands are designed to allow moderators to control Nightbot within chat. We offer the ability to change spam protection settings, manage regulars, and manage custom commands – all within chat. To give moderators more control, they can be [added as a manager](https://docs.nightbot.tv/control-panel/managers) of the channel to get control panel access.

### Default Commands List

* [!commands](https://docs.nightbot.tv/commands/commands)
  Allows users to see a list of channel commands, and allows moderators to manage custom commands
* [!filters](https://docs.nightbot.tv/commands/filters)
  Allows moderators to manage spam protection filter settings
* [!game](https://docs.nightbot.tv/commands/game)
  Allows users to see the current game of the stream, and allows moderators to change the current game
* [!poll](https://docs.nightbot.tv/commands/poll)
  Allows moderators to create a Strawpoll within chat, and allows users to see the results
* [!regulars](https://docs.nightbot.tv/commands/regulars)
  Allows moderators to manage the channel regulars list
* [!songs](https://docs.nightbot.tv/commands/songs)
  Allows users to request songs, and allows moderators to manage the requested songs queue
* [!title](https://docs.nightbot.tv/commands/title)
  Allows users to see the current title of the stream, and allows moderators to change the current title
* [!winner](https://docs.nightbot.tv/commands/winner)
  Allows moderators to choose a random active user as a winner.

### Managing Default Commands

To manage default commands, head to the [default commands page](https://beta.nightbot.tv/commands/default) in the control panel.

A table of default commands will be shown, along with their status and buttons for managing their functionality.

You can disable commands you do not wish to use by clicking on the "Disable" button towards the right of a default command listed in the table, and vice versa for enabling.

There is also an options button that will allow you to change the userlevel and cooldown of default commands.

- *Userlevel* - Selects who has the permission to execute the command. For example, selecting “Regulars” allows users in your channel's regular list the permission to use the command. Larger channels may want Userlevel set to Regulars or above.

- *Cooldown* - Time minimum amount of time between command uses (to prevent the command from spamming the chat)

## Custom Commands

Nightbot is able to be programmed with customized commands which can be utilized to display information to your chatroom. Most frequently this is social links, but there is a multitude of cool commands you can form.

For example, if a popular streamer is consistently bombarded by requests for a link to their YouTube channel, they may create a command which links directly to their YouTube channel. Instead of having to manually type or say it each time, just simply calling the command in chat will display the link.

### Creating Custom Commands

To create custom commands, click on the "Add Command" button on your [commands page](https://beta.nightbot.tv/commands/custom).

Then, fill in the form with your desired command name, message, userlevel, and cooldown.

- *Command* - Generally speaking, commands are usually prefixed with exclamation points. They can in fact be anything you would like, or even none at all. Command names are not allowed to contain spaces.

- *Message* - The response of the command. You can use [Variables](https://docs.nightbot.tv/commands/variables) in your messages to make dynamic messages.

- *Userlevel* - Selects who has the permission to execute the command. For example, selecting “Regulars” allows users in your channel's regular list the permission to use the command. Larger channels may want Userlevel set to Regulars or above.

- *Cooldown* - Time minimum amount of time between command uses (to prevent the command from spamming the chat)

### Removing and Editing Existing Commands

The control panel makes it a breeze to edit and delete existing custom commands. On the commands page, a list of created custom commands will be shown in a table. Under the actions column are buttons for editing and deleting commands.

Use the pencil button to edit existing command. It will bring up a form similar to when adding a command.

Use the trash can button to remove a command.

### Editing Custom Commands in Chat

It is also possible to manage commands within chat. Check out the [!commands](https://docs.nightbot.tv/commands/commands) default command documentation for instructions on doing that.
