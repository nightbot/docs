/*
Title: ToUser
*/

The touser variable just prints the first parameter given to a command.

## Usage

> $(touser)

#### Example Usage

> $(touser)

would result in

> nightdev

if the first parameter after the command was nightdev

## Examples

#### Adding a command to hug a user

> !commands add !hug /me hugs $(touser)