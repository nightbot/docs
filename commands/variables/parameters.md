/*
Title: Parameters
*/

The parameters variables (1-9) print parameters split by spaces after a command. This is primarily useful when used within nested commands.

## Usage

> $(`number`)

`number` can be a value from 1 through 9

## Example

> $(3)

would print the third parameter after a command.

If the input for a !command was

> !command lorem ipsum dolor

the result would be dolor