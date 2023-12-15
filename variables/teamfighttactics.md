/*
Title: TeamfightTactics
*/

You can use the TeamfightTactics variable to create commands that display rank information for a Riot ID.

## Usage

> $(teamfighttactics `riot_id` `region`)

`riot_id` is the Riot ID being looked up (`GameName#TagLine`)
`region` is the region the summoner plays on

#### Example Usage

> $(teamfighttactics testing#1234 na)

would result in

> testing#1234's current rank: Challenger I

## Examples

#### Adding a command to show chatters your rank

> !commands add !rank $(teamfighttactics `riot_id` `region`)

#### Adding a command to allow users in chat to lookup their own account

> !commands add !rank $(teamfighttactics $(query))

### Legal Jibber Jabber

Nightbot isn’t endorsed by Riot Games and doesn't reflect the views or opinions of Riot Games or anyone officially involved in producing or managing Teamfight Tactics. Teamfight Tactics and Riot Games are trademarks or registered trademarks of Riot Games, Inc. Teamfight Tactics © Riot Games, Inc.
