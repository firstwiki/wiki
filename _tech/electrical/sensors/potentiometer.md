---
title: Potentiometer
tag: sensors
---

{% include cleanup %}

A **potentiometer**, also called a **pot**, is an analog sensor that changes resistance in
proportion to the position of its shaft. Potentiometers can found in rotary or
linear varieties. In a rotary potentiometer, the shaft rotates and causes the
change in resistance. In a linear (or slide) potentiometer, the shaft moves in
a straight line. Potentiometers can also come in audio or linear tapers. The
audio taper means that the output varies logarithmically with the position of
the shaft, and is useful for volume knobs in audio equipment. In linear taper
pots, the output varies linearly. The concept of tapers and shaft arrangements
are independent, a linear potentiometer can have a audio taper, and vice
versa.

## Usage

In [FIRST Robotics](first), when wiring the pot, one end of the potentiometer is
connected to 5V and the other end to ground. The sense line is connected to the
analog input on the [Robot Controller](robot-controller). Thus, the
potentiometer acts as a voltage divider, where the values of the two resistors
can be varied.

Potentiometers can also be wired directly to Talon SRX or Jaguar [motor
controllers](speed-controller).

Potentiometers are used, therefore, to determine where specific moving parts
are in their range of travel on the robot, or to provide analog input to the
[Operator Interface](operator-interface).

{% include historical %}

Note that when working with analog values on the [2004 Robot
Controller](robot-controller-2004), the function `Get_Analog_Value` must first
be called. This is not necessary when the pot is connected to the Operator
Interface.
