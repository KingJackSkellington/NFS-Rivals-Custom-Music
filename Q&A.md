## "Why do we have to use an MP3 file specifically? Why not .WAV, .OGG, .FLAC, etc.?"
* The dandev-el3.exe can only convert MP3 files. Trying to convert any of the above formats will result in a 1KB file and outputting an error in the Command Prompt.
-----
## "I see that Frosty Editor lets me import an MP3/WAV file already. Why bother converting it in the first place?"
* When importing either an MP3 or WAV file, Frosty Editor will encode the audio to the "Pcm16Big" codec.
* If you go ahead and try to play the music in-game this way, it will unfortunately result in the audio being cut off thoughout the entire playback.
* As of the writing of this guide, the current version of Frosty Editor (1.0.6.3) doesn't allow you to change codecs to avoid this issue.
* Using the dandev-el3.exe file to convert it to .ealayer3 circumvents this issue.
-----
## "I have multiple music mods installed. Will they all play?"
* No. Frosty Mod Manager will only play the music mod that is highest in the load order, and will discard the rest.
