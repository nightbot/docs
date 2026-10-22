---
title: "Weather"
---

You can use the weather variable to create commands that display weather information for a specific location.

## Usage

> $(weather `location`)

`location` is the location being looked up. It can be a city name, a city with a state or country (such as `Paris, Texas` or `London UK`), or a US ZIP code, Canadian postal code, or UK postcode.

#### Example Usage

> $(weather Austin TX)

would result in

> Weather for Austin, Texas, United States: Conditions are Clear with a temperature of 71F (22C). The wind is blowing from the ENE at 3mph (5km/h) and the current humidity is 49%.

## Examples

#### Adding a command to show chatters your local weather

> !commands add !weather $(weather `location`)

#### Adding a command to allow users in chat to lookup their own weather

> !commands add !weatherlookup $(weather $(query))

## Data Sources

Weather data is based on data from [MET Norway](https://api.met.no/), licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). Temperatures and wind speeds are converted to imperial and metric units.

Locations are resolved using data from [GeoNames](https://www.geonames.org/), licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
