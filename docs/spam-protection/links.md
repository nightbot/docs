---
title: "Links"
sidebar_position: 4
---

Nightbot offers a link filter that allows you to control how links are handled in your chat.

## Usage

Managing Links can be found in the Nightbot Spam Protection menu by owners and channel managers. This filter can also be managed through the [!filters command](https://docs.nightbot.tv/commands/filters).

To view settings for Nightbot's links filter, head over to the [Spam Protection menu](https://nightbot.tv/spam_protection).

Clicking the Options button will open a popout that you can customize filter settings.

## Advanced Usage

### Regex

The links filter also supports regular expressions (regex) for more whitelist options. You can enter a regex expression with the pattern below.

> `~/[pattern]/[flags]`

### Example

`~/i.imgur.com\/[\d\w]+.(png|jpg|gif)/i` will whitelist imgur direct links such as ([i.imgur.com/ghOCjsn.png](https://i.imgur.com/ghOCjsn.png)), but will not allow image links ([imgur.com/ghOCjsn](https://imgur.com/ghOCjsn)), gallery links, and album links ([imgur.com/a/Tkyl6](https://imgur.com/a/Tkyl6)).

#### Options

- *Link Whitelist* - This is the list of allowed links, entered one entry per line. You can allow entire websites (example: `youtube.com`) or specific links (example: `twitter.com/nightbotapp`).

- *Timeout Length* - This is the maximum length of time Nightbot will timeout users for when being punished for this spam filter. Nightbot always issues a warning for first offenses (either the message is deleted or the user is timed out for 5 seconds), and repeat offenses yield the length you select. The 600-second default value is equivalent to 10 minutes.

- *Exempt Userlevel* - This is the minimum required userlevel to be exempt from this filter. For example, if `regular` is set, regulars are able to post links and not get punished.

- *Silent Mode* - Enable this setting and Nightbot will no longer give messages to punished users. This is useful for busier channels where Nightbot floods the chat with timeout explanation messages.

- *Custom Message* - This sets a custom message to be displayed to users when they are punished from the links filter. Leaving this blank will use the default messages, which are randomly chosen Duke Nukem quotes.

### Permitting Links

Users can be temporarily permitted to post a link using the !permit command. The [!filters command](https://docs.nightbot.tv/commands/filters) needs to be enabled for the !permit to function.

#### Usage

> !permit night

will allow the user night to post links for the duration of 60 seconds.

### Managing Links

All filters can be managed through the [Spam Protection menu](https://nightbot.tv/spam_protection) or through the [!filters command](https://docs.nightbot.tv/commands/filters).
