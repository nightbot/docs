/*
Title: PSN
*/

You can use the PSN variable to create commands that display trophy information about a specific PSN profile.

## Usage

> $(psn `username`)

`username` is the Playstation Network ID being looked up

#### Example Usage

> $(psn night)

would result in

> NIGHT has a level of 1 and currently has 0 platinum, 0 gold, 0 silver, and 0 bronze trophies.

## Examples

#### Adding a command to show chatters how many trophies you have

> !commands add !psn $(psn `username`)

#### Adding a command to allow users in chat to lookup their own account

> !commands add !psnlookup $(psn $(query))