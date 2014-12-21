Moving Automation
=================

Moving a Region to a new location will not automatically move the
Automation data that might be aligned with it, as we can see in the
following screen shots.

![01.move\_automation](static/Ardour-MovingAutomation-01-move_automation-en.png "01.move_automation")

![02.move\_automation](static/Ardour-MovingAutomation-02-move_automation-en.png "02.move_automation")

Dragging Automation
-------------------

Using the "*Control*" or "*Apple*" key while dragging moves the current
Automation point in any direction, and also all subsequent points
horizontally only. This may provide a way to move groups of Automation
points to the new Region location in certain situations.

![03.move\_automation](static/Ardour-MovingAutomation-03-move_automation-en.png "03.move_automation")

Consolidating the Region with Processing
----------------------------------------

However, dragging the Automation points independent of the Region may
not be accurate enough in many circumstances. To preserve a Region with
the Automated processing of the Fader, Panning and Plugins preserved, it
is necessary to Consolidate the Region with the processing.

First, set the Automation to "*Play*".

![04.1.move\_automation](static/Ardour-MovingAutomation-04-1-move_automation-en.png "04.1.move_automation")

Next, with the appropriate Track selected, create a Range with the Range
tool and Right-Click to get the Range options menu. Then, select
"*Consolidate range with processing*".

![04.move\_automation](static/Ardour-MovingAutomation-04-move_automation-en.png "04.move_automation")

This creates a new Region with the Automated processing applied to it.
The new Region containing this Automated processing will appear on the
same Track and place in the Timeline, replacing the previous,
unprocessed Region. The original Region is still preserved in the
Regions List in case it is needed elsewhere.

![05.move\_automation](static/Ardour-MovingAutomation-05-move_automation-en.png "05.move_automation")

Be sure to use the "*clear*" button in the Automation section to remove
the previous automation. Then the newly consolidated Region can be moved
to the desired location.

![06.1.move\_automation](static/Ardour-MovingAutomation-06-1-move_automation-en.png "06.1.move_automation")

Bouncing the Region with Processing
-----------------------------------

Another option is to use the "*Bounce range to the regions list with
processing*" option, also available from the Range options Right-Click
menu.

![](/ardour3/http://en.flossmanuals.net/floss/pub/Ardour/MovingAutomation/)![](http://en.flossmanuals.net/floss/pub/Ardour/MovingAutomation/)![07.move\_automation](static/Ardour-MovingAutomation-07-move_automation-en.png "07.move_automation")

This creates a new Region, with all of the processing included, in the
Regions list. You can then create a new Track, here shown as "*Audio
2*", and drag the new Region ("*Audio 1.1-0-bounce-5*") to that Track.
As can be seen here, the original Region is left unchanged in the
"*Audio 1*" Track.

![08.move\_automation\_1](static/Ardour-MovingAutomation-08-move_automation_1-en.png "08.move_automation_1")

Drawing Gain Automation
-----------------------

Another type of Automation was introduced in the **Changing Edit Modes**
chapter. This tool, the **Draw Gain Automation** tool, is found in the
Edit Modes menu, and can also be used by typing the keyboard shortcut
*"G".*

![004.automation](static/Ardour-EditModes-004-automation-en_1.png "004.automation")

Use this tool if you want to draw Region-specific volume **Automation**.
When this Cursor Mode is selected, your cursor pointer will look like
this:

![004.automation.icon](static/Ardour-EditModes-004-automation-icon-en_1.png "004.automation.icon")

With this tool, Region Gain Automation can be drawn directly in the
Region itself, unlike Fader Automation which is drawn or recorded in the
Automation track. Region Gain Automation is separate from, and in
addition to, Fader Automation.

As with the Automation Tracks, a **Gain Automation Point** can be
dragged in any direction with the mouse. To remove a Gain Automation
Point, hold down the "*Shift*" key while Right-Clicking on it.

![09.move\_automation](static/Ardour-MovingAutomation-09-move_automation-en.png "09.move_automation")

The Automation created in this way will stick to the Region on which it
was created, even when the Region is moved around.

![10.move\_automation](static/Ardour-MovingAutomation-10-move_automation-en.png "10.move_automation")

This type of gain Automation is drawn directly on the Region itself,
which makes it different from the Automation used in the drop-down
Automation region (see chapter on **Using Automation**).

Deactivating and Removing Gain Automation
-----------------------------------------

Gain Automation can be reset or deactivated from the Region context
menu, which is reached by Right-Clicking on the Region. Here, the Gain
Automation is referred to as the **Envelope**. In this menu, you have
the options of "*Reset Envelope*", which removes the Gain Automation
Points you have drawn in the Region, "*Envelope Visible*", which toggles
visibility of the Gain Automation on and off (leaving it active however)
and "*Envelope Active*", which toggles whether the Gain Automation is
active or not (but leaves it visible). An inactive but visible Envelope
is blue rather than green.

![automation\_new.01](static/Ardour-MovingAutomation-automation_new-01-en.png "automation_new.01")

Continuing
----------

By now you should have a complete Session ready, with Regions, Tracks,
Mixing, Plugins and Automation all in place. The only thing left to do
now is to Export your Stereo Mix to an audio file which you can listen
to, burn as a CDR or convert to an MP3/OGG to share on a website. Please
continue on to the next section, **Exporting Sessions**, to learn the
different ways of doing this.
