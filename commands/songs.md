/*
Title: !songs
Sort: 8
*/

The !songs command is used to manage Song Requests within Nightbot. **Note**: Make sure [song requests](https://beta.nightbot.tv/song_requests) are enabled before using these commands.

## Viewing Current Song

### Usage 

> !songs current

will display the title of the current song. 

### Example

> !songs current

will display the current song

> Night -> "AWOLNATION - Sail (Official Music Video)" by Red Bull Records is the current song.

## Deleting Queued Song

### Usage 

> !songs delete `queue_postion`

will delete the song at the current `queue_postion`.

### Example

> !songs delete 2

will delete the song in the 2nd postion and return

> Night -> The song has been removed.

## Getting List of Songs

### Usage 

> !songs list

will give a link to view all song requests.

### Example

> !songs list

will return the response

> Night -> The song list for this channel is available at https://beta.nightbot.tv/t/night/song_requests

## Getting Channels Playlist

### Usage

> !songs playlist

will return a link to the the channels playlist

### Example

> !songs playlist

will return the response

> Night -> The song playlist for this channel is available at https://beta.nightbot.tv/t/night/song_requests/playlist

## Getting Next Song

### Usage 

> !songs next

will display the next requested song. This is also `queue_postion` 1.

### Example

> !songs next

will display the next song

> night -> "AWOLNATION - Run (Audio)" by Red Bull Records is the next song.

## Requesting a Song

### Usage 

> !songs request `Youtube or SoundCloud Link / Search Term`

Will use the link or search term supplied to add a song to the queue. **If YouTube or SoundCloud has been disabled in the song request settings, they cannot be used to request songs.**

### YouTube

YouTube videos can be requested with the whole YouTube link, the video ID (text after `/watch?v=`), or through a search term (if YouTube is the selected search provider).

#### Usage

These chat commands will all result in the same song added to the song queue.

> !songs request https://www.youtube.com/watch?v=ngzC_8zqInk

> !songs request ngzC_8zqInk

In the case of search terms

> !songs request Arctic Monkeys - R U Mine?

will search YouTube for a video with the closest name if the channel configured YouTube as the search provider. 

**Note**: When entering the video ID only the standalone ID will work. No additional charaters can be added, for example `!songs request /watch?v=ngzC_8zqInk` and `!songs request ?v=ngzC_8zqInk` will result in an error.

### SoundCloud

SoundCloud tracks can be requested with the whole SoundCloud link or through a search team if SoundCloud is the selected search provider.

#### Usage

> !songs request https://soundcloud.com/johnlegend/all-of-me-3

In the case of search terms

> !songs request All of me - John Legend

will search SoundCloud for a track with the closest name if the channel configured SoundCloud as the search provider.

## Skipping Current Song

### Usage 

> !songs skip

will skip the current song.

### Example

> !songs skip

will the skip current song and return

> Night -> "AWOLNATION - Sail (Official Music Video)" by Red Bull Records has been skipped.

## Promoting a Song

### Usage 

> !songs promote `queue_postion`

will move the song in the `queue_postion` to postion 1; the next song.

## Editing Song Volume

### Usage 

> !songs volume `between 1 - 100`

will change the current volume to the specified number.

### Example

> !songs volume 32

will set the volume to 32 and return

> Night -> The volume has been updated to 32.