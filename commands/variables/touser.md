/*
Title: ToUser
*/

The touser variable just prints the first argument given to a command.

## Usage

> $(touser)

#### Example Usage

> $(touser)

would result in

> nightdev

if the first argument after the command was nightdev

#### Example Usage

if **no** argument after the command

> $(touser)

would result in

> night

if the current executer of the command was night

## Examples

#### Adding a command to hug a user

> !commands add !hug /me hugs $(touser)
