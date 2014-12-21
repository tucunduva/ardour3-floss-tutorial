Ardour: UsingSendsAndInserts

Using Sends
===========

In Ardour, you can add **Sends** to Tracks and Busses. Also called
Auxilliary Sends (Aux Sends), in Ardour they are simply Processors in a
bus or track channel strip. Sends tap the signal at a specific point in
the signal flow (pre-fader, post-fader, before or after EQs and other
plugins, etc.) and send a copy of that signal somewhere else, without
affecting the normal signal flow downwards to the channel fader.

In summary, a Send is just an extra output for a Track or Bus with its
own Fader that can be used to route the signal to other points in
Ardour.

When is a Send useful? \
------------------------

To add a particular effect to a set of Tracks without creating multiple
instances of the same Plugin, one approach would be to create a Bus, add
one instance of the effect Plugin to the Bus, and Route the outputs of
multiple Tracks to that Bus. This applies the effect equally to all
routed Tracks and the "clean" (unprocessed) signal of these tracks is no
longer available.

A more flexible approach is to use Sends. To do this, create a Bus with
the desired Plugin, then add a Send in each track to which you want to
apply the effect. Next, Route the Send outputs to the Bus. Now you can
use the Send Faders to control how much of each Track's signal is sent
to the effect Bus Plugin. Using this approach, the 'clean' signals from
each Track remain available to the Master Mix. Because Sends are very
useful for this kind of work with effect Plugins, they are also commonly
called "Effect Sends".

Creating and Using a Send 
--------------------------

This section will show how to create and use a Send in the manner
described above. First create a Bus, name it appropriately, and add a
Plugin in the Pre-Fader Region (right-click just above the Fader blue
rectangle in the Processor Box), as discussed in the chapter **Using
Plugins**.

### Creating the Bus and adding a Plugin

In this example, we have created a Mono Bus called "*DRUMS*", and added
the "*Freeverb*" Reverb LADSPA Plugin to the bus.

![](static/Ardour3_Sends_1.png) \

The "-" display in the Bus Input-Routing button indicates that nothing
is routed to this bus yet. Before routing a send to this Bus first make
sure that the Bus outputs are Routed to the Master Bus, as shown below
(button at bottom reads "*master*").

![](static/Ardour3_Sends_2.png) \

Also, open the Plugin Window and set the Plugin's signal mix to 1.0 Wet
Level and 0.0 Dry Level. \

![](static/Ardour3_Sends_3.png) \

This ensures that the Bus carries all of the processed signal (the 'Wet'
signal) from the Plugin, and none of the unprocessed signal (the 'Dry'
signal) to the Master Bus. Remember, the unprocessed, 'clean' signals
are still available from their original tracks, so there is no need to
duplicate them in this Bus.

### Creating and Routing Sends \

Now we can create Sends in the other Tracks and route them to the Bus
inputs.

Like Plugins, Sends are also created in the Processor Box. Go to each of
your drum tracks, right-click on the Processor Box, and create a New Aux
Send directed to the appropriate Bus (in our case, named DRUMS). \

![](static/Ardour3_Sends_4.png) 

 

It is important to consider whether you want to create a Pre-Fader or
Post-Fader Send. Generally this depends on the type of effect Plugin
used and the desired result.

in the same Pre-Fader Regions and Post-Fader Regions above and below the
Fader where Plugins are inserted. In Pre-Fader Sends, the Send Level is
controlled only by the Send Fader, independently of the Track/Bus Fader.
In Post-Fader Sends, the Send Level is controlled by both the Track/Bus
Fader *and* the Send Fader. This means that the Post-Fader Send level is
always proportional to the Track/Bus level, which controls the 'Dry'
signal.  \

To create Post-Fader Sends, Right-Click in the Post-Fader area below the
Fader in one of the Audio Tracks and select **New Send ...**

![Create a new
Send](static/Ardour-UsingSendsAndInserts-Create_New_Send_1-en.png)

This creates a new Send and pops up the Send Output Routing Editor
window. Since this is a Stereo Track, first add 2 outputs and then
connect each output to the corresponding input of the previously created
Reverb Bus.

![Routing\_send\_Output\_1\_1](static/Ardour-UsingSendsAndInserts-Routing_send_Output_1_1-en.png "Routing_send_Output_1_1")

When a new Send is created, it is deactivated by default. When a Send is
not active, its name is shown in parentheses. In order to actually send
signal out, the Send must first be activated. Right-click on the Send
and select Activate.

![Activate a
Send](static/Ardour-UsingSendsAndInserts-Activate_Send_1-en.png)

To give the Send a more appropriate name, Right-Click on it and select
**Rename**. This pops up a little rename window.

![Rename\_Send\_1\_1](static/Ardour-UsingSendsAndInserts-Rename_Send_1_1-en.png "Rename_Send_1_1")

Now our new Send is activated (note that the parentheses have
disappeared) and ready for action.

![Acive\_and\_Renamed\_send\_1.png](static/Ardour-UsingSendsAndInserts-Acive_and_Renamed_send_1-en.png)

To control the Send level, double-click on the Send to open the Send
window.

![Send\_Window\_1\_1](static/Ardour-UsingSendsAndInserts-Send_Window_1_1-en.png "Send_Window_1_1")

The Fader on the left controls how much of this Track's signal is sent
to the Reverb Bus. Since this is a Post-Fader Send, this Send level is
proportional to the actual (clean) Track level as set by the Track
Fader.

Continuing
----------

Now that you know how to **Add Plugins** to a Track, as well as how to
**Add Sends** to Tracks to create Plugin Busses usable by any number of
Tracks, it might be helpful to learn about a few other Plugins useful in
the Mixing Process. Please continue on to the following chapters
covering **Dynamics** and **Equalizing**.
