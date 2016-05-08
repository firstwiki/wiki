---
title: Jaguar Motor Controller
tags: speed-controller
---

{% include stub %}

The **Jaguar** is a [speed controller](speed-controller) developed by Luminary
Micro and supplied by Texas Instruments. The Jaguar was added to the FIRST
Robotics Competition in the 2010 season to supplement the [Victor
884](victor-884). It has had two different versions, the MDL-BDC "Grey Jaguar"
and the MDL-BDC24 "Black Jaguar".


## Technical

The Jaguar is part of the FIRST [control system](Control_system
"Control system" ). The Jaguar works by recieving a [PWM
signal](pwm-signal) or
[CAN](can) input from a [robot
controller](Robot_controller "Robot controller" ), which may
include the (full) [Robot Controller](Robot_Controller "Robot
Controller" ), the [Robovation](Robovation "Robovation" )
controller or a [Vex](Vex "Vex" ) Controller. Depending on the
range of the [PWM](PWM "PWM" ) signal - with 0 being full reverse,
127 being neutral, and 254 being full forward - the Victor 884 adjusts the
output of the motor accordingly. This achieves a variable speed control for
such applications as [drivetrains](Drive_trains "Drive trains" ),
arms, or elevators.

The nominal operating voltage of the MDL-BDC is 12 volts, while the MDL-BDC24
is capable of 24 volt operation as well. Both have a maximum operating current
of 40 amps.

