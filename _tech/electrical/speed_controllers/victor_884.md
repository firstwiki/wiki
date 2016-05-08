---
title: Victor 884
tags: speed-controller
---

{% include historical %}
{% include outdated-warning %}

The **Victor 884** is a [speed controller](speed-controller) developed by [Innovation FIRST](innovationfirst) as an improved version of the [Victor
883](victor-883). The Victor 884 works by reading a
[PWM](pwm) signal from a [robot
controller](robot-controller), and adjusting
the effective voltage supplied to the motors accordingly. The Victor 884 was
the only FIRST legal speed controller allowed in the
[2005](triple-play) [control
system](control-system).


## Technical

The Victor 884 was part of the FIRST [control system](control-system).
The Victor 884 works by recieving a [PWM
signal](pwm-signal) input from a [robot
controller](robot-controller), which may
include the (full) [Robot Controller](robot-controller), the [Robovation](robovation)
controller or a [Vex](vex) Controller. Depending on the
range of the [PWM](pwm) signal - with 0 being full reverse,
127 being neutral, and 254 being full forward - the Victor 884 adjusts the
output of the motor accordingly. This achieves a variable speed control for
such applications as [drivetrains](drive-trains),
arms, or elevators.

The operating voltage of the Victor 884 ranges from 6V to 15V DC, with a
maximum operating current of 40 amps. The variable output from the Victor 884
ranges from 3% to 100% of full throttle. A cooling fan operated by the input
voltage of the speed controller insures that the Victor 884 is continuously
cooled.


### Use

Although some motors may be run on a [Spike](spike-relay) if desired, the [CIM
motors](cim-motor) must use a Victor 884 speed controller. The Victor 884 Speed
Controllers may be wired into either a 30 Amp or 40 Amp fuse on the breaker
panel depending on the motor being used. Each additional motor on a FIRST
Competition Robot needs to have a Victor 884 or [Spike relay](spike-relay).


### Coast/Brake

A small jumper on the Victor 884 determines whether the Victor will 'coast' or
'brake' when it stops receiving signal. In 'coast' mode, momentum of the
spinning motor will enable the motor to coast to a stop when it stops
receiving signal. In 'brake' mode, the Victor will short the output terminals
together, providing a resistance to the momentum of the spinning motor. As
such, the motor will come to a stop much more quickly.

Typically, a robot will use 'coast' mode on most drive motors, as abrupt stops
can cause tipping issues. Turrets, arms, and other manipulators should usually
use 'brake' mode, both to help hold a load at its desired position and to aid
in controllability.


## Connections


### Data

A 3-pin [PWM cable](pwm_cable) connects the Victor 884 to the [robot
controller](robot-controller). On the Robot Controller, the PWM cable destined
for the Victor 884 speed controller should be connected to the "PWM output" set
of ports. A relay extension cable] or a Y-cable may be used if the Victor is
mounted far away from the Controller or if one wants a single PWM output port on
the Controller to control multiple Victors.


### Input

The two input terminals on the Victor supply the
power needed to run the speed controller, the cooling fan, and the motor
output. The cooling fan on the Victor 884 should be wired into the two input
terminals. This insures that the speed controller stays cool whenever the
Victor is on. If wired incorrectly to the output terminals, the cooling fan
will only work when the output motor is being driven, which will lead to over
heating and the possible release of [magic smoke](magic-smoke).

The two input wires must be correctly wired to match their polarity. If the
polarity of the input wires is switched, the speed controller may cease to
function. Sparks, arcing, fire, burning smells, or [magic smoke](magic-smoke)
may indicate that a Victor 884 was wired incorrectly, and hence has also been
destroyed.


## Programming

The PWM outputs on
the [Robot Controller](robot-controller) can be
set across the normal hobby servo range, 1 to 2 ms. The 8-bit PWM channels
used on the PIC microprocessor of the Robot Controller (and Vex controller)
has a resolution of 256 values, which fit in an `unsigned char`. Zero commands
full reverse, 127 commands stop, and 254 commands full forwards. The command
255 should be avoided on older RCs because it acts as a special signal command
when transmitted between the Robot Controller and OI. Newer versions of the RC
seem to have no issue with a 255 command. However, for code portability, 254
should be the maximum value used (besides, using 254 results in symmetric
forward and reverse resolutions).

Note that a neutral PWM command to a factory calibrated Victor consists of a
pulse of about 1.5 ms duration. As such, when no PWM input is applied, the
Victor will detect this and flash it's LEDs yellow.

