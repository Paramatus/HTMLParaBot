# Para-Simple-Gif-Bot
A simple Gif Bot that takes chat commands and plays a Gif on command

## Shoutout
Thanks to Instafluff for the ComfyJS Library

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

The Gif play duration is also measuret in Milliseconds and can be changed by changing the playTime varaible

Default:
```
playTime: 4500
timeout: 180000
```
