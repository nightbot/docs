/*
Title: !poll
Sort: 6
*/

The !poll command allows you and your moderators to easily create polls using [Straw Poll](https://strawpoll.me/). Only 1 poll can be active at one time.

## Creating a Poll

### Usage

> !poll new `title` | `option_1` | `option_2`

`title` is main title of your poll.

`options` are the indivual options your users can vote for spilt by a vertical bar `|`, 2 options are required, however a maximum of 30 can be added.

### Example

> !poll new Should I bake a pizza? | yes | no | maybe

Will create a poll with 3 options to vote on and display a link in the chat. The command will return.

> Night started a new poll: "Should I bake a pizza?" - Head to `https://strawpoll.me/#######` to vote!

## Viewing Results

### Usage

> !poll results

This command will output the current poll and display vote values.

### Examples

> !poll results

will return in chat

> StrawPoll Results: yes: 5 vote, no: 3 votes, maybe: 4 votes