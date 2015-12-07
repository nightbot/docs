/*
Title: Query
*/

The query variable prints anything a user types after a command. This is useful when combined with other variables that accept parameters.

## Usage

> $(query)

## Examples

#### Adding a command to show the weather

> !commands add !weather $(weather $(query))

#### Adding a command to lookup an Xbox Live gamertag

> !commands add !xbl $(xbl $(query))