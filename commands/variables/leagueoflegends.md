/*
Title: LeagueOfLegends
*/

You can use the LeagueOfLegends variable to create commands that display rank information for a summoner name.

## Usage

> $(leagueoflegends `summoner_name` `region` `queue`)

`summoner_name` is the summoner name being looked up

`region` is the region the summoner plays on (values can be `br`, `eune`, `euw`, `jp`, `kr`, `lan`, `las`, `na`, `oce`, `tr`, `ru`, and `pbe`)

`queue` is an optional parameter for the queue type to search for (values can be `ranked_tft`, `ranked_solo_5x5`, `ranked_flex_sr`, and `ranked_flex_tt`)

#### Example Usage

> $(leagueoflegends testing na)

would result in

> Testing's current rank: Silver III

## Examples

#### Adding a command to show chatters your rank

> !commands add !rank $(leagueoflegends `summoner_name` `region` `queue`)

#### Adding a command to allow users in chat to lookup their own account

> !commands add !rank $(leagueoflegends $(query))

### Legal Jibber Jabber

Nightbot isn’t endorsed by Riot Games and doesn't reflect the views or opinions of Riot Games or anyone officially involved in producing or managing League of Legends. League of Legends and Riot Games are trademarks or registered trademarks of Riot Games, Inc. League of Legends © Riot Games, Inc.
