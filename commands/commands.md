/*
Title: !commands
*/

The !commands command allows users to get a link to your custom commands page and allows you and your moderators to add, remove, and modify custom commands.

## Adding Commands

### Usage

> !commands add `!command_name` `command response`

`!command_name` is the name of command you wish to use. Commands are usually prefixed with an exclamation mark.

`command response` is the message you want Nightbot to reply with when the command is called.

### Example

> !commands add !testing this is a test message

When !testing is called, the command will return "this is a test message"

## Editing Commands

### Usage

> !commands edit `!command_name` `command response`

`!command_name` is the name of command you wish to edit.

`command response` is the message you want Nightbot to reply with when the command is called.

### Example

> !commands edit !testing new testing message

When !testing is called, the command will now return "new testing message"

## Deleting Commands

### Usage

> !commands delete `!command_name`

`!command_name` is the name of command you wish to use.

### Example

> !commands delete !testing

## Advanced Usage

When adding and editing commands, the user level required to execute a command as well as the command's cool down length can be modified. You just need to apply the parameters as shown below.

> !commands add `!command_name` -ul=`userlevel` -cd=`cooldown` `command response`

Replace `!command_name` and `command response` as normally, and then replace `userlevel` with a valid userlevel from below. Replace `cooldown` with the minimum number of seconds you want between command uses.