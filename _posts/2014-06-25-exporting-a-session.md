Exporting Sessions
==================

**Exporting** is the process of saving a Region, Track or Session to a
file on your computer which you can listen to, burn as a CDR or convert
to an MP3 to share on a website. As we learned previously, Exporting a
Region does not Export all of the changes you might have made to that
Region. To Export edits such as **Normalizing**, **Fading** and
**Panning**, and **Automation**, you must Export either a Range or the
entire Session. \

To Export a Session, use the top menu: *Session \> Export \> Export
session to audiofile.*

Everything included between the "start" and "end" Location Markers in
the Timeline will be Exported, so you have to set the markers first if
they are not in the correct position. \

![sessions01.png](static/Ardour-Export-sessions01-en.png)

Since the Export is handled through the Master Bus, all the Tracks
within the Range you select will be Exported together, exactly as they
play back in your Session. Unlike the Export Region command, this kind
of Export includes any Normalizing, Fading and Panning, and Automation
you have created, along with the individual edits made to the Regions as
well. If any of the Tracks have the Mute or Solo buttons engaged, this
will also affect which Tracks will be heard in the Exported file. \

This will open up a dialogue box with several options. You'll want to
export a Stereo mix, usually as an **AIFF** or **WAV** file, at either
**16-bit** or **24-bit**. 16-bit files can be burnt directly to an audio
CD, but if you intend the audio to be further processed, it is best to
export it at 24-bit. Having chosen your options, enter the track name at
the top and select *Export*.

Define the Output channels by clicking the check boxes in the section on
the right. Left and Right are normal Stereo outputs.

![exportrange3.png](static/Ardour-Export-exportrange3-en_1.png)

To export only specific Tracks, de-select the master outs, and click the
”Specific tracks” button and select the channel(s) of the Track(s) you
wish to Export.

![exportrange4\_1](static/Ardour-Export-exportrange4_1-en_1.png "exportrange4_1")\

*Warning: overwriting existing files causes Ardour to become confused,
resulting in empty files being Exported. Be sure to use a unique file
name each time you Export!*

![exportregion4\_1.png](static/Ardour-Export-exportregion4_1-en_2.png)

Continuing
----------

At the end of this Session, you now have an Exported Stereo Mix
representing your entire Session. You're almost finished! The only thing
left to do is save the Ardour Session itself. There are a number of ways
to do this, and we will discuss them in the following section, **Saving
Sessions**. \


