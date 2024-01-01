/*
Title: Blacklist Words/Phrases
Sort: 1
*/

Nightbot offers a blacklist filter that allows you to set timeouts for custom words, phrases, and patterns.

## Usage

Creating and Managing Blacklist Words and Phrases can only be done by the owner and channel managers in the Nightbot Spam Protection menu.

### Adding to a Blacklist

To add words and phrases to Nightbot's Blacklist head over to the [Spam Protection menu](https://nightbot.tv/spam_protection).

Clicking the Options button will open a popout that you can customize blacklist settings.

## Advanced Usage

### Regex

The blacklist filter also supports regular expressions (regex) for more filtering options. You can enter a regex expression with the pattern below.

> `~/[pattern]/[flags]`

### Example

`~/(\d{3}[-.])?\d{3}[-.]\d{4}/` will blacklist any like looking phone numbers such as 253.532.8757 and 321-2345.

#### Options

- *Blacklist* - This is the text box of filtered words and phrases you wish to blacklist. Entering one entry per line. You can use an asterisk (\*) as a wildcard character to dynamically filter words and phrases. For example, `test*` blocks `test`, `testing`, `testerino`, etc.

- *Timeout Length* - This is the maximum length of time Nightbot will timeout users for when being punished for this spam filter. Nightbot always issues a warning for first offenses (either the message is deleted or the user is timed out for 5 seconds), and repeat offenses yield the length you select here. The 600-second default value is equivalent to 10 minutes.

- *Exempt Userlevel* - This is the minimum required userlevel to be exempt from this filter. For example, if `regular` is set, regulars are able to use blacklisted words and not get punished.

- *Silent Mode* - Enable this setting and Nightbot will no longer give messages to punished users. This is useful for busier channels where Nightbot floods the chat with timeout explanation messages.

- *Custom Message* - This sets a custom message to be displayed to users when they are punished from the blacklist filter. Leaving this blank will use the default messages, which are randomly chosen Duke Nukem quotes.

### Managing Blacklist Filter

All filters can be managed through the [Spam Protection menu](https://nightbot.tv/spam_protection) or through the [!filters command](https://docs.nightbot.tv/commands/filters).
