/*
Title: User
*/

The user variable just prints the current user using the command.

## Usage

> $(user)

#### Example Usage

> $(user)

would result in

> nightdev

if the current executer of the command was nightdev

## Examples

#### Adding a command to make Nightbot hug the command caller

> !commands add !hugme /me hugs $(user)