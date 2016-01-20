/*
Title: !filters
Sort: 4
*/

The !filters command allows you and your moderators to edit existing Nightbot filters. For managing filters in the control panel please see [Spam Protection](https://docs.nightbot.tv/control-panel/spam-protection).

## Selecting Spam Filter

### Usage

> !filters `spam_filter`

As explained above, the filters command at its core allows control over Nightbot's spam protection filters.

`spam_filter` is the name of the filter that you or your moderators wish to manage and edit. The current spam filter names are identical to the [Spam Protection](https://docs.nightbot.tv/control-panel/spam-protection) located in the Control Panel. The filter names are as followed:  

- **blacklist** - Prevents chatters from posting certain words or phrases [[*more info*](https://docs.nightbot.tv/spam-protection/blacklist)]
- **caps** - Prevents chatters from posting in all or mostly capitalizes messages [[*more info*](https://docs.nightbot.tv/spam-protection/caps)]
- **emotes** - Prevents chatters from posting many emotes in messages [[*more info*](https://docs.nightbot.tv/spam-protection/emotes)]
- **links** - Prevents chatters from posting links, and allows you to whitelist certain links [[*more info*](https://docs.nightbot.tv/spam-protection/links)]
- **symbols** - Prevents chatters from posting many symbols in messages [[*more info*](https://docs.nightbot.tv/spam-protection/symbols)]

As this step alone Nightbot will return both if the filter is enabled or disabled and further spam protection settings that can be managed.

### Example

> !filters caps

will return the response

> Night -> No setting was specified. Current status for caps filtering: enabled. Possible settings: enable/disable/limit/message/time/silent/userlevel

## Filter Management 

### Usage

> !filters `spam_filter` `settings`

After specifying a `spam_filter` from above, entering a setting will allow you and your moderators to modify certain aspects of the specified filter. The settings are identical to those in the [Spam Protection](https://docs.nightbot.tv/control-panel/spam-protection) menu.

After selecting a setting you want to modify, a value, such as a number or text, needs to be entered to change the setting.

**Note**: Placing "enable" or "disable" in the setting will turn on and off the specified filter respectively.

### Examples

These examples show an assortment of different use cases for the !filter command.

> !filters caps limit 8

will change the current limit of caps before timeout to 8

> !filters links message No Links!

will change the links timeout message to "No Links!"

> !filters symbols disable

will disable the symbols filter timeout functionality entirely

