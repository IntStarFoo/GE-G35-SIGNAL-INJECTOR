GE-G35-SIGNAL-INJECTOR
======================

A board layout that enables an easy process for tapping into the POWER, GROUND, SIGNAL wires in a GE G35 LED light set.  The goal is to create a simple, safe and switchable link between the original signal a new signal produced by whatever proc is plugged in.  And Stuff.

I give no guarantees of safety or function.  Use at your own risk.


<h3>Feature Considerations</h3>
The main goal is to be able to leave the original operation features intact with the option of physically switching the signal over to the output from your own MCU.  

I wanted to stick to a single sided, single layer design so people could more easily manufacture the board at home, but it may be a bit too complex for that.  If there is an option to sending the layout to an online board house and ordering 3 or 4 for a reasonable price, that works too.


<h4>Basic 2 way switch</h4>
Position 1 completely disconnects the additional MCU and routes the signal from the original controller to the signal line running through the bulbs.  
Position 2 completely disconnects the original signal from the original controller and replaces it with a the signal coming from a pin on the additional MCU.
<h5>Possible Additional Features</h5>
There may also be a case where someone wants to intercept the signal from the original controller and feed it into the additional MCU for further processing.  I'm not sure if this should be an additional position on the mechanical switch or connected via a jumper.
There may also be a case where someone wants to use a relay in place of the mechanical switch.  If it's possible to design the PCB in such a way that the switch option and relay option are available, then great. 


<h3>Physical Layout Considerations</h3>
I've been thinking about ways to simplify installation onto a set of lights.   I am a little apprehensive about this part because of the possibility for someone to incorrectly attach the wires.  This connector design might also be helpful for replacing / removing bad bulbs. That process is a pain and currently requires cutting out the section containing the bad bulb and reconnecting the two bare ends.

I configured this for the MSP430.  I'm not sure how popular the 20 pin style MCU socket is and how common it is to have the 3 connections required (ground, power, signal) located in the pin positions.  Thoughts and feedback here are much needed.


Options include: 

1. A crimp-on tap connector similar to an automotive wire tap.  The tap connector would have to perform an additional, advanced maneuver where it actually severs the middle (signal) line as it is crimped on.  Also, there would have to be some method for dealing with crimping it on in either direction. (V+, Signal, GND) vs (GND, Signal, V+).  I believe there are some simple circuits that could auto correct for polarity.  

2.  A PCB with screw block connectors and wire holders (see drawing below).

A suggestion was made to make the input and output screw terminal positions... _"pcb routing might be a little easier with the screw terminals side by side, especially if you're willing to reverse the wire order, which it seems you are."_
<img src="http://i.imgur.com/sJBjPhM.jpg">

Current Schematic (Last updated by svenstucki)<br/> 
<img src="http://i.imgur.com/YQDnRil.png">
Current Layout (Last updated by svenstucki)<br/>
<img src="http://i.imgur.com/ONy1fNW.png">

Example Board Completed (with scrap parts)<br/>
<img src="http://i.imgur.com/rHGEp4G.jpg"><br/>
<img src="http://i.imgur.com/Si5ACyE.jpg"><br/>
