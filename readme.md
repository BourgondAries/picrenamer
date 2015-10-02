# Picrenamer #

To use this program, run it from the directory containing what you want to sort out.
Anything with an extension that can not be identified is put in a not_pictures folder.
The program will open a picture viewer and focus the terminal, prompting you for a new name.
The renamed object is put into the renamed/ folder in the current working directory.
If it already exists, the file will _not_ be overwritten.
If you do not enter any new name, it will be put in the folder skipped/.

## Inner Workings ##
The script can be edited, the standard image viewer is eom, and the media player is vlc.
The first two lines define these. Both of them are killed when renaming is complete.
There should be a more elegant method.

Another thing is that a subshell is started that continuously focuses the renaming terminal.
This is to avoid vlc or eom to gain foreground control.
