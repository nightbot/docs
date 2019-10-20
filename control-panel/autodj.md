/*
Title: AutoDJ
Sort: 4
*/

AutoDJ is the player responsible for Song Requests with Nightbot.

## Usage

The [AutoDJ](https://nightbot.tv/song_requests) page contains Song Request settings, a music player with media controls, and a queue of upcoming songs. The controls at the top of the page are as follows: 

- *Enable & Disable* - This setting will enable or disable new requests from being put in the queue.
- *Clear Queue* - Will clear all songs currently in the queue.
- *Add Song* - Will open a popup where you can enter a direct url (from SoundCloud or Youtube) or search term for the defined Search Provider.


### Settings

The Settings control opens a popup where all settings are divided into three categories. These settings can only be changed in the Control Panel.

#### General

- *Userlevel* - This is the minimum required userlevel to request a song. Userlevels are listed from highest to lowest.
- *Providers* - Services you wish to allow users to request songs from. You can check and uncheck different music providers.
- *Playlist* - When your song request queue is empty, songs are pulled from the selected playlist. "Channel" is your own [personal playlist](https://nightbot.tv/song_requests/playlist).
- *Search Provider* -  This is the provider that you want to be used for searching songs. Users can add songs by entering the URL or by searching the selected search provider. 

#### Limits

- *Queue Length* - This is the maximum amount of songs that can be stored in the queue. This can be between 1 - 100 songs.
- *Limit to Playlist* - Enabling this will force songs requested to originate from the playlist selected under general.
- *User Limit* - This is the maximum amount of songs that a user can request at a time.
- *Exempt Userlevel* - This is the minimum required userlevel to be exempt from the user limit. Userlevels are listed from highest to lowest. The userlevel is still affected by the Queue Length and cannot go beyond the limit.

#### YouTube

This category is dedicated to [YouTube](https://www.youtube.com) available controls.

- *Limit to Music* - This will require requested YouTube videos to be from the Music category.
- *Limit to Liked Videos* - This will only allow people to request YouTube videos with more likes than dislikes to help reduce lower content videos.

### Player Controls & Song Information

The music player will change automatically in accordance to the selected Providers in the Settings. For example from, YouTube to SoundCloud, depending on the requested song site.

#### Controls

- *Play & Pause* - Used to play or pause the currently playing song.
- *Next Song* - The next song button can be used to instantly start the next queued song.
- *Track Slider* - Used to display the current location of the song and can be used to jump around on the current song.
- *Volume* - Used to change the overall volume of AutoDJ, also controllable through the [!volume](https://docs.nightbot.tv/commands/songs#editing-song-volume) command.

#### Song Information

The music player will also give the following information while the song is currently playing:

- Song/Video Title - Uploader
- Song Duration
- Link to Song
- User Who Requested Song
- Save to Channel Playlist Button

### Queue

Below the player and controls lays the queue where AutoDJ displays the upcoming songs.

Using the gray up arrow icon you can promote a song to be first in the queue. To delete upcoming songs use the red trash icon on the right of the entry. Both of these can also be done with the [!songs](https://docs.nightbot.tv/commands/songs) command.

Gray colored songs in the queue are playlist entries set in the Settings. The playlist will play if the queue is empty and will allow newly requested songs to be played next.