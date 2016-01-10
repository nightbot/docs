/*
Title: !songs request
Sort: 9
*/

Requesting songs is the sole part of Nightbot Song Requests. This guide is how to request songs in Nightbot AutoDJ streams. There are currently two places to requests songs, in the stream chat ([!songs](https://docs.nightbot.tv/commands/songs)) command and in the channel songlist page. For a guide on playing songs please see the [AutoDJ](https://docs.nightbot.tv/control-panel/autodj) guide.

To get a link the songlist page of the channel use the command `!songs list`. The songlist page shows current songs in the queue and allows you to request songs right from the page!

Below are the current song providers that songs can be requested from and that channel owners can choose from.

## YouTube

YouTube videos can be requested with the whole YouTube link, the video ID (text after `/watch?v=`) or through a search term (if YouTube is the selected Search Provider).

### Usage

These chat commands will all result in the same song added to the song queue.

> !songs request https://www.youtube.com/watch?v=ngzC_8zqInk
> !songs request ngzC_8zqInk

In the case of search terms

> !songs request Arctic Monkeys - R U Mine?

will request a YouTube video of that search if the owner has YouTube as the Search Provider. 

**Note**: When entering the video ID only the standalone ID will work. No additional charaters can be added, for example `!songs request /watch?v=ngzC_8zqInk` and `!songs request ?v=ngzC_8zqInk` will result in an error.


## SoundCloud

SoundCloud tracks can be requested with the whole SoundCloud link, or through a search team (if SoundCloud is the selected Search Provider).

### Usage

> !songs request https://soundcloud.com/johnlegend/all-of-me-3

In the case of search terms

> !songs request All of me - John Legend

will request the SoundCloud track of that search if the owner has SoundCloud as the Search Provider.

**Note**: Because of the full link request, `soundcloud.com` may need to be added as a Link Whitelist in the [Links Spam Protection](https://docs.nightbot.tv/spam-protection/links).