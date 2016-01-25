/*
Title: League of Legends
*/

You can use the League of Legends variable to create commands that display rank information for a summoner name.

## Usage

> $(leagueoflegends `summoner_name` `region`)

`summoner_name` is the summoner name being looked up
`region` is the region the summoner plays on

#### Example Usage

> $(leagueoflegends testing na)

would result in

> testing's current rank: Challenger I

## Examples

#### Adding a command to show chatters your rank

> !commands add !rank $(leagueoflegends `summoner_name` `region`)

#### Adding a command to allow users in chat to lookup their own account

> !commands add !rank $(leagueoflegends $(query))