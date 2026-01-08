---
title: "!poll"
sidebar_position: 6
---

The !poll command allows you and your moderators to easily create polls using [Straw Poll](https://strawpoll.com/).

## Creating a Poll

### Usage

> !poll new `title` | `option 1` | `option 2`

`title` is the main title of your poll.

`options` are the individual options your users can vote for. Split by a vertical bar `|`, 2 options are required, however, a maximum of 30 can be added.

### Example

> !poll new Should I bake a pizza? | yes | no | maybe

will return a new StrawPoll with options yes, no, and maybe:

> Night started a new poll: "Should I bake a pizza?" - Head to https://strawpoll.com/ABC123def456 to vote!

## Viewing Results

### Usage

This command will output the most recent poll's results

> !poll results

### Example

> !poll results

will return

> StrawPoll Results: yes: 5 votes, no: 3 votes, maybe: 4 votes
