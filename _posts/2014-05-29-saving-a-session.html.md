Saving Sessions
===============

There are a number of ways to save Sessions in Ardour, so that each
Session can be use later on. The simplest way is to save the entire
Session as a single Ardour file.

Save a Session \
----------------

You can save your session by pressing *"Control"* + *"S"* (or *"Apple"*
+ *"S"* on OS X), or by using the menu *Session \> Save*.

![sessions02.png](static/Ardour-saving-sessions02-en.png)

Ardour File & Folder Format
---------------------------

A typical Session's folder on your hard drive might look something like
this:

    2009-11-25T20:03:10.ardour      interchange
    2009-11-25T20:03:10.history     looping2.ardour
    analysis                        looping2.ardour.bak
    dead_sounds                     looping2.history
    export                          looping2.history.bak
    instant.xml                     peaks

The name of this Session is "*looping2*". The first entries, listed here
as

    2009-11-25T20:03:10.ardour
    2009-11-25T20:03:10.history

are a timestamped Snapshot of the Session and its history. Ardour will
use this Snapshot to recover from a crash.

The folder named *export* is often used for Exporting files from your
Session.

A Session file has the *.ardour* extension. The Session file is
periodically backed up by Ardour with a *.bak* extension.

    looping2.ardour
    looping2.ardour.bak

The *.history* file keeps a record of changes you have made during your
Session, and is also periodically backed up.

    looping2.history
    looping2.history.bak

The *interchange* folder contains the actual audio data of all the
Regions used in your Session.

    $ ls interchange/looping2/audiofiles/
    Audio 1-1%L.wav
    Audio 1-1%R.wav
    cheesy synth-1%L.wav
    cheesy synth-1%R.wav
    cymbal-0-bounce-1.wav
    cymbal-1.wav
    guitar_drone.edit1.wav
    highhat-0-bounce-1.wav
    highhat-1.wav
    kick-0-bounce-1.wav
    kick-1.wav
    slap bass 2-1.wav
    slap bass-1.wav
    snare-0-bounce-1.wav
    snare-1.wav

And finally, the *peaks* folder contains the data Ardour uses to
graphically display the Peaks of your soundfiles.

    $ ls peaks/
    cymbal-0-bounce-1%A.peak
    guitar_drone.edit1%A.peak
    guitar_drone.edit1%B.peak
    highhat-0-bounce-1%A.peak
    kick-0-bounce-1%A.peak
    snare-0-bounce-1%A.peak
    teeeest%A.peak
    teeeest%B.peak
    teeeest2%A.peak
    teeeest2%B.peak

Continuing
----------

Saving an entire Session allows you to open it again at a later time.
However, if you would like to preserve a certain state that your Session
is in, to be able to return to that state later on after you have made
changes, then please continue to the next session called **Saving
Snapshots**. \

