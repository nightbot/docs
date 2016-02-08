/*
Title: Links
Sort: 4
*/

Nightbot offers Links filters that allows you to control how Links are handled in your chat.

## Usage

Managing Links can be found in the Nightbot Spam Protection menu by owners and channel managers. This filter can also be managed through the [!filters command](https://docs.nightbot.tv/commands/filters).  

To view settings for Nightbot's links filter, head over to the [Spam Protection menu](https://beta.nightbot.tv/spam_protection). 

Clicking the Options button will open a popout that you can customize filter settings.

#### Options

- *Link Whitelist* - This is the list of allowed links, entered one entry per line. You can allow entire websites (example: `youtube.com`) or specific links (example: `twitter.com/thenightbot`).

- *Timeout Length* - This is maximum length of time Nightbot will timeout users for when being punished for this spam filter. Nightbot always issues a 5 second timeout for first offenses, and repeat offenses yield the length you select. The 600 second default value is equivalent to 10 minutes.

- *Exempt Userlevel* - This is minimum required userlevel to be exempt from this filter. For example if `regular` is set, regulars are able to post links and not get punished. 

- *Silent Mode* - Enable this setting and Nightbot will no longer give messages to punished users. This is useful for busier channels where Nightbot floods the chat with timeout explanation messages.

- *Custom Message* - This sets a custom message to be displayed to users when they are punished from the links filter. Leaving this blank will use the default messages, which are randomly chosen Duke Nukem quotes.

### Managing Links

All filters can be managed through the [Spam Protection menu](https://beta.nightbot.tv/spam_protection) or through the [!filters command](https://docs.nightbot.tv/commands/filters).