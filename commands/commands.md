/*
Title: !commands
Sort: 3
*/

The !commands command allows users to get a link to your custom commands page and allows you and your moderators to add, remove, and modify custom commands.

## Adding Commands

### Usage

> !commands add `!command_name` `command response`

`!command_name` is the name of command you wish to use. Commands are usually prefixed with an exclamation mark

`command response` is the message you want Nightbot to reply with when the command is called

### Example

> !commands add !testing this is a test message

When !testing is called, the command will return

> this is a test message

## Editing Commands

### Usage

> !commands edit `!command_name` `command response`

`!command_name` is the name of command you wish to edit

`command response` is the message you want Nightbot to reply with when the command is called

### Example

> !commands edit !testing new testing message

When !testing is called, the command will now return

> new testing message

## Deleting Commands

### Usage

> !commands delete `!command_name`

`!command_name` is the name of command you wish to use

### Example

> !commands delete !testing

## Advanced Usage

### Userlevels and Cooldowns

When adding and editing commands, you can also specific the userlevel required to execute the command as well as the command's cooldown time. You just need to apply the parameters as shown below.

> !commands add `!command_name` -ul=`userlevel` -cd=`cooldown` -a=`!alias` `command response`

`!command_name` / `command response` is the same as above.

`cooldown` is the minimum number of seconds between command uses.

`userlevel` is one of the valid userlevels from below.

`!alias` is a different command you want this command to call. Note that the input passed to the provided alias is the `command response`. To capture user input, you'd need to place [variables](https://docs.nightbot.tv/commands/variables) in the `command response` (like `$(query)`).

#### UserLevel values

* **owner** - Channel Owner
* **moderator** - Channel Moderator
* **regular** - Nightbot Regular (users in the [regulars](https://docs.nightbot.tv/control-panel/regulars) list)
* **subscriber** - Paid Channel Subscriber
* **everyone** - Normal User *(default)*

### Variables

Variables can be used within command responses. For a list of variables and examples of their use, check out the [Variables](https://docs.nightbot.tv/commands/variables) page.
