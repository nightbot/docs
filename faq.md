/*
Title: Nightbot FAQ
Sort: 3
*/

Here is are the most common questions we get asked, all on one page. If you still need more support for specific items use the [Nightbot Forum](https://community.nightdev.com/c/nightbot) or use the [Contact Form](https://www.nightdev.com/contact/) for a more private matters.

## Why isn't Nightbot joining, I'm using Youtube Gaming? Why is Nightbot taking a long time to respond on Youtube Gaming?

Nightbot for YouTube will only join your channel when you are live and it can take a few minutes for it to join after you go live. This is currently a limitation on YouTube due to rate limits on YouTube's API.

Youtube uses a another way to send and receive messages and because of these limitation it will take Nightbot some time to receive your message. The more active your chat is the faster the response. If your chat is inactive/slow, it could take Nightbot 2 minutes to respond due to polling limitations. 

Both of these limitations cannot be worked around. If Nightbot still isn't joining your channel, it's either not a moderator in your channel or is banned from your channel.

## My Playlist was deleted and I can't find it. How do I get it back?

Navigate to the [AutoDJ settings](https://beta.nightbot.tv/song_requests) and under the **General** Header change the **Playlist** setting to **Channel**. Your playlist can be edited in the [Playlist](https://beta.nightbot.tv/song_requests/playlist) page.

If the above doesn't show your playlist please use the [Contact Form](https://nightdev.com/contact/) as you playlist may not have transfered correctly.

Why do I get songs in AutoDJ that I can't delete? Why can't it be my playlist instead?

This is because you have another playlist active in the AutoDJ settings. Please refer to the question right above this to change this.

## How do I get the current song to display on OBS/XSpilt?

In order to achieve this you need to use the [Nightbot Application](https://docs.nightbot.tv/app-beta). This will create a text file with the current song playing in the `%USERPROFILE%\Documents\Nightbot\` location on Windows and in the `/Users/USERNAME/Documents/Nightbot/` on OSX. At the current time there is no way to edit the output of the song, this will be added in the future releases.

## This isn't working and it should be. This should be added to Nightbot!

While that isn't a question, we are always looking to remove bugs from Nightbot. Without someone reporting them they can often go unnoticed. In order to report a bug do it from the [Contact Form](https://nightdev.com/contact/) or using the [forum](https://community.nightdev.com/c/nightbot). If you have a feature that you think should be added tell us on the forum! We're always looking for ways to make Nightbot to improve. 
