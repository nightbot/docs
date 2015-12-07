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

## Examples

#### Adding a command to hug a user

> !commands add !hug /me hugs $(touser)