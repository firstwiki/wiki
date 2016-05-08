---
title: Sensors
---

{% include outdated-warning %}

A **sensor** is a device that detects, or _senses_, the surrounding environment.
In terms of robotics, and specifically [FIRST](first), sensors enable the
[robot](robot) to better understand what is around it and how to react. The
types of sensors used in FIRST are electrical, meaning that they send signals to
the [Robot Controller](robot-controller) that is then converted into some value
for use by the program. There are two main classes of sensors, [analog](analog)
and [digital](digital). An analog sensor, such as a
[potentiometer](potentiometer), will have a value in the range of 0 to 1023 (10
bits). A digital sensor, such as a [limit switch](limit-switch), is much more
limited, only having _off_ and _on_ states, represented by 0 and 1.

Sensors are important aspects of [programming](Programming "Programming" ),
allowing truly complex robots that can react intelligently to dynamic
situations. The use of advanced sensors is often necessary to develop an
effective [autonomous mode](autonomous-mode), though many other uses are
possible. Sensors can count the number of rotations of a particular wheel and
then the program can adjust speed based on this information; sensors can
determine whether some apendage is fully extended, and then shut off power to a
motor; sensors can allow the robot to avoid objects that the robot
[operator](operator) might not see.

Each year the list of sensors included with the [kit of parts](kit-of-parts)
varies, but here are examples of sensors that were included in prior kits of
parts.

  * [IR sensor](ir-sensor)
  * Banner sensor
  * [Gyroscope](gyroscope)
  * [Current sensor](current-sensor)
  * [Pressure sensor](pressure-switch)
  * [Accelerometer](accelerometer)
  * A vision system such as [CMUcam2](cmucam2). 
  * [Encoder](encoder)

See electronics rules for the current year's game for information on where and
which sensors may be bought, and the price limit on them.
