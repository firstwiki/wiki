---
title: Pressure Switch
tags: pneumatics
---

A **pressure switch** is a [pneumatics](pneumatics)
switch whose state changes depending on the pressure.


## Data

Sends a digital signal. The two terminals are shorted together when the
pressure is greater than 95psi after hitting a peak of 115psi. The terminals
are disconnected when the pressure is less than 115psi after dropping below
95psi.


## Connections


### Air

Connects to the system via a 1/8" NPT thread on the bottom.


### Signal

Two terminals on the top that are connected to a digital input on the robot
controller, connecting on the black and white wires.


## Current Product Info

{% include outdated-warning %}

### Supplier

* Supplied by [[The Nason Company](http://www.nasonptc.com
"http://www.nasonptc.com" )].


### Model Number

SM-2B-115R


## Programming

The Robot Controller needs to check the pressure switch and react accordingly
by applying power to the compressor when needed. [WPILib](wpilib) contains a 
compressor object that will do this automatically for you.

