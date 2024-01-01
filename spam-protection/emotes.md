/*
Title: Emotes
Sort: 3
*/

Nightbot offers a emotes filter that allows you to control how excessive Twitch emotes are handled in your chat.

## Usage

Managing excessive emotes can be found in the Nightbot Spam Protection menu by owners and channel managers.

To view settings for Nightbot's emotes filter, head over to the [Spam Protection menu](https://nightbot.tv/spam_protection).

Clicking the Options button will open a popout that you can customize filter settings.

#### Options

- *Timeout Length* - This is the maximum length of time Nightbot will timeout users for when being punished for this spam filter. Nightbot always issues a warning for first offenses (either the message is deleted or the user is timed out for 5 seconds), and repeat offenses yield the length you select. The 600-second default value is equivalent to 10 minutes.

- *Limit* - This is the minimum number of emotes before Nightbot will punish the user for spamming. The default limit is 3 emotes.

- *Exempt Userlevel* - This is the minimum required userlevel to be exempt from this filter. For example, if `regular` is set, regulars are able to use excessive emotes and not get punished.

- *Silent Mode* - Enable this setting and Nightbot will no longer give messages to punished users. This is useful for busier channels where Nightbot floods the chat with timeout explanation messages.

- *Custom Message* - This sets a custom message to be displayed to users when they are punished from the emotes filter. Leaving this blank will use the default messages, which are randomly chosen Duke Nukem quotes.

### Managing Emotes Filter

All filters can be managed through the [Spam Protection menu](https://nightbot.tv/spam_protection) or through the [!filters command](https://docs.nightbot.tv/commands/filters).
