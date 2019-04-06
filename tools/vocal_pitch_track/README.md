# Vocal Pitch Tracker

[Related TouchDesigner Forum Thread](http://derivative.ca/Forum/viewtopic.php?f=22&t=11467&p=57324&hilit=pitch#p57324)

This is a quick and dirty pitch detection COMP that returns the fundamental frequency in Hz and associated note name for a vocal input. It simply looks for the first spectral peak over the 'Peak Threshold'. It outputs when the RMS of the input signal is over the 'Trigger Threshold'. These parameters are of course both dependent on your microphone/audio input.

Needed one for testing and didn't see anything in the forum. It's all OPs and commented. Hopefully it's of use!

**Update v.2:**
Tested with additional microphones. Made a few minor tweaks to the data output. 
Now returns additional note information via out1 CHOP:
freq - frequency in Hz
note - note number within octave
octave - octave number
midi - midi note number

out2 DAT returns note name.
