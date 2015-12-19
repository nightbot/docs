/*
Title: Count
*/

The count variable prints how many times a command has been used.

## Usage

> $(count)

#### Example Usage

> $(count)

would result in

> 1

if this was the first time you called the command, then

> 2

The next time you called the command, and so on

## Examples

#### Adding a command to show how many hugs Nightbot has given

> !commands add !hug /me hugged $(touser) ($(count) hugs have been given)