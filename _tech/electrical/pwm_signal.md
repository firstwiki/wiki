---
title: PWM Signal
---

{% include stub %}

A PWM signal, pulse-width-modulated signal, is an analog output value
used to control motors through [Victors](victor) or
[Jaguars](jaguar).


## Programming

On the [robot controller](robot-controller), a PWM signal has a range from -127
to 127 in where -127 corresponds to full power "backwards" on the motor and 127
to full power "forwards" on the motor. Some controllers may use a range from -1
to 1 with the same actions occurring at the minimums and maximums of the range.
Zero is neutral in both cases and does not move send any current to the motor
(though the [Victor](victor) or [Jaguar](jaguar) can change what exactly happens
at this signal).


## External Links

  * [Explanation of PWM Signals](https://learn.sparkfun.com/tutorials/pulse-width-modulation)
