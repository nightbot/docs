/*
Title: !poll
Sort: 6
*/

The !poll command allows you and your moderators to easily create polls using [Straw Poll](https://strawpoll.me/).

## Creating a Poll

### Usage

> !poll new `title` | `option 1` | `option 2`

`title` is main title of your poll.

`options` are the indivual options your users can vote for spilt by a vertical bar `|`, 2 options are required, however a maximum of 30 can be added.

### Example

> !poll new Should I bake a pizza? | yes | no | maybe

will return a new StrawPoll with options yes, no, and maybe:

> Night started a new poll: "Should I bake a pizza?" - Head to https://strawpoll.me/6369092 to vote!

## Viewing Results

### Usage

This command will output the most recent poll's results

> !poll results

### Example

> !poll results

will return

> StrawPoll Results: yes: 5 vote, no: 3 votes, maybe: 4 votes
