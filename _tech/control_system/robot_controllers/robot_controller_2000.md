---
title: Robot Controller (2000)
tags: [robot-controllers, obsolete-part]
---

{% include historical %}

The 2000 RC was a big upgrade from the older system. It used a
[BS2sx](BS2sx) to replace the [BS2](BS2). This was also the first one designed and manufactured by
[InnovationFIRST](InnovationFIRST). It was used
for the 2000-2002 seasons (and with minor modifications for the 2003 season).

The 2000-2003 Robot Controller systems consisted of three processors. The
[Operator Interface](operator-interface) used
a [PIC16F877](PIC16F877) microcontroller to collect
data from all the digital and analog inputs and communicate with the Robot
Controller via a radio or tether. The second processor was the user processor,
a Basic Stamp 2SX. The User Processor was the only user-programmable CPU in
the entire system. The third processor, the Master Processor, was a PIC16
microcontroller, which controlled the outputs for all relays, speed
controllers, and other output devices. The General-purpose IO pins of the
BS2SX were not accessible as they were connected to LEDs on the controller
itself. The only direct connection available to the BS2SX was the "programming
port", two pins on the Stamp normally dedicated to RS232 communication with
the host programming PC.

The 2000-2003 Robot Controllers were programmed in [PBASIC](PBASIC), a [Parallax](Parallax)-dialect of
[BASIC](http://www.wikipedia.org/wiki/BASIC "wikipedia:BASIC" ). Program flow
was very similar to modern code,
with a main loop and similar timing characteristics involved. Code would first
have to declare all variables used, which were bits, nibbles, bytes, or words.
Then initialization of the master processor would occur. The Stamp would use
SHIFTOUT to establish communication with the Master Processor and bring the
entire stack online. Then, the main loop would start. In the main loop, a long
SERIN instruction would collect all input data from the Input microprocessor.
The user code would manipulate the data as it saw fit, and then would use
SEROUT to pipe the data to the Master microprocessor. This is roughly
analogous to the current GetData() and Put_Data() in the PIC control
system. Even the timing is nearly identical--both systems were required to
output data ever 26.2 ms.


## External links

  * [InnovationFirst.com](http://innovationfirst.com "http://innovationfirst.com" )
  * [Documentation for 2001 through 2003 Control Systems](http://innovationfirst.com/FIRSTRobotics/documentation-legacy.htm "http://innovationfirst.com/FIRSTRobotics/documentation-legacy.htm" ). 
