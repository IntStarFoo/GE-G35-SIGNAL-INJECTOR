GE-G35-SIGNAL-INJECTOR
======================

A board layout that enables an easy process for tapping into the POWER, GROUND, SIGNAL wires in a GE G35 LED light set.  The goal is to create a simple, safe and switchable link between the original signal a new signal produced by whatever proc is plugged in.  And Stuff.

I give no guarantees of safety or function.  Use at your own risk.


I've been thinking about ways to simplify installation onto a set of lights.   I am a little aprehensive about this part because of the possibility for someone to incorrectly attach the wires.  This connector design might also be helpful for replacing / removing bad bulbs.

Options include: 

1. A crimp-on tap connector similar to an automotive wire tap.  The tap connector would have to perform an additional, advanced manuever where it actually severs the middle (signal) line as it is crimped on.  Also, there would have to be some method for dealing with crimping it on in either direction. (V+, Signal, GND) vs (GND, Signal, V+).  I believe there are some simple circuits that could auto correct for polarity.  

2.  A PCB with screw block connectors and wire holders (see drawing below).

A suggestion was made to make the input and output screw terminal positions... _"pcb routing might be a little easier with the screw terminals side by side, especially if you're willing to reverse the wire order, which it seems you are."_
<img src="http://i.imgur.com/sJBjPhM.jpg">
