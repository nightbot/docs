---
title: "Weather"
---

You can use the weather variable to create commands that display weather information for a specific location.

## Usage

> $(weather `location`)

`location` is the location being looked up

#### Example Usage

> $(weather kappa)

would result in

> Weather for Kappa, IL: Conditions are Overcast with a temperature of 37 F (3 C). The wind is blowing From the South at 15 MPH and the current humidity is 100%.

## Examples

#### Adding a command to show chatters your local weather

> !commands add !weather $(weather `location`)

#### Adding a command to allow users in chat to lookup their own weather

> !commands add !weatherlookup $(weather $(query))