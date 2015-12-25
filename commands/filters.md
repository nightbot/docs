/*
Title: !filters
Sort: 4
*/

The !filters command allows you and your moderators to edit existing Nightbot filters. For using filters in the control panel please see [Spam Protection](https://docs.nightbot.tv/control-panel/spam-protection).

## Usage

> !filters `filter_name` `setting` `[value]`

`filter_name` is the name of the filter you wish to edit. Current filter names include `blacklist`, `caps`, `emotes`, `links`, and `symbols`.

`setting` is the setting that you wish to edit under your `filter_name`. Current settings include `enable`, `disable`, `limit`, `message`, `time`, `silent`, and `userlevel`. 

`[value]` is the optional value that is needed when changing certain settings such as `limit`, `message`, `time`, `silent` and `userlevel`. The values can be true or false, whole number, or a string depending on what is required.

### Example

> !filters caps limit 8

Will set the limit of caps before timeout to 8. 

> !filters blacklist

Will show current status of blacklist filter and show possible settings. 

> !filters links message No Links!

Will change the links timeout message to "No Links!".

> !filters symbols disable

Will disable the symbols filter entirely.