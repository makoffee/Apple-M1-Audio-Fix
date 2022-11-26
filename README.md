# Apple M1 Audio Fix
Script to temporarally address Apple Macbook Pro M1 audio problems such as pops, distortion, and crackling.

## Issue ##
2021 Macbook Pro users have documented audio issues such as popping sounds, distorted crackling while durring audio playback.  Issue seems not to be related to any kind of problem with the speaker, but instead is related to heavy memory usage and poor handeling of audio buffer size during playback under heavy CPU and memory load.  This issue has been well documented on the following communities:

- https://discussions.apple.com/thread/253531295
- https://developer.apple.com/forums/thread/132423?page=11
- https://www.reddit.com/r/macbookpro/comments/qmpg3k/2021_macbook_pro_speakers_crackling_and_popping/


* Note: Many of the offered solutions are uneducated guess, particully the suggestions to manimulate MIDI audio clock rates have no effect on this issue. *

## Temporary fix ##
Removing corrupted audio preferences, and killing coreaudiod. After getting tired of typing these commands, I've created a small script to run these two actions, as the issue will occur multiple times a day. Restarting the system after running the script seems to keep the audio issues from coming back so quickly.

## Usage ##
- Download 'fixaudio.sh'
- Make script executable in terminal with command 'chmod +755 fixaudio.sh'
- run './fixaudio.sh'
- enter your password
- enjoy no more popping sounds
- (optional) reboot your system

That's it.  I hope Apple will find a fix for this, and publish an update soon.
