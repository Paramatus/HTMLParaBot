# Para-Simple-Gif-Bot
A simple Gif Bot that takes chat commands and plays a Gif on command

## Shoutout
Thanks to Instafluff for the ComfyJS Library (https://www.github.com/instafluff/ComfyJS)

## Setup
Download and edit the GifBot.html file so that "ChannelName" is replaced with your channel name in lower case letters. Then you have to add a browser source in OBS or XSplit and use local file and add the GifBot.html

## Align the gif to a corner
To align the Gif you have to eidt the Custom CSS from 
```
body { background-color: rgba(0, 0, 0, 0); margin: 0px auto; overflow: hidden; }
```
to 
```
body { background-color: rgba(0, 0, 0, 0); margin: 0px auto; overflow: hidden; position:absolute; bottom:0; right:0; }
```
to make the gif appear in the bottom right corner. Just remove the "bottom:0" or the "right:0" to make it align to the corner you want to or leave it empty to make it align to the top left corner.

## Change Gif play time and timeout between Gifs
To change the Timeout, that someone has to wait to play a gif, you have to change the variable Timeout. It is measured in milliseconds

The Gif play duration is also measured in Milliseconds and can be changed by changing the playTime varaible

Default:
```
playTime: 4500
timeout: 180000
```
##Commands
| Command  | Discription |
| ------------- | ------------- |
| !gif | Plays the personal Gif of a User |
| !adduser [username] [gif Link]  | Adds or updates a personal gif for a User  |
| !removeuser [username] | Removes the gif of a User  |

#Advanced Bot
The GifBotAdvanced gives the opportunity to play sound effects, while the give is playing. It also requires a view more information when adding a User. (The Setup is still the same)

## Commands

| Command  | Discription |
| ------------- | ------------- |
| !gif | Plays the personal Gif of a User |
| !adduser [username] [gif Link] [display time of the gif] [soundlink (must end on .mp3)] [volume (0.0 - 1.0)]   | Adds or updates a personal gif for a User every variable after the gif link is not mandatory for a gif to show up.  |
| !removeuser [username] | Removes the gif of a User  |
| !setvolume [username] [volume (0.0 - 1.0)] | Updates the volume of the the soundeffect for a specific User |
| !picture [picture link] [time in seconds] | Added Mod show picture, which allows a mod to display a picture on stream for a certain amount of time |
## Side Note
Yes, the display duration is not a set Value anymore and is must not be modified when adding a User because it will get set to 4500ms when not set. But do not leave out variables that are in between other variables. 