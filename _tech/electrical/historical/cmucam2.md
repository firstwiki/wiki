---
title: CMUCam2
---

{% include historical %}
{% include stub %}


The **CMUcam2** is a vision system given to teams in the [kit of
parts](kit-of-parts), starting in
[2005](triple-play).

The camera communicates with the [full robot controller](robot-controller) via
the TTL port, with an TTL/RS-232 converter and buffer provided by [Innovation
First](innovation-first). The camera is commonly mounted to two servos in order
to locate objects.


## Purpose

The camera is used to track a colored object.

In [2005](triple-play), colored pieces of plastic were used. These did not work
too well, as the camera was very sensitive to their angle, and the amount of
light.

In [2006](aim-high), the camera has a green target that is lit by six lights.
This ensures that the lighting conditions do not effect the ability of the
camera too much.


## Camera Mount

The camera came with a pan and tilt mount powered by servos that could be used
to allow the robot to "look around". The mount also made it easy for teams to
mount the camera on their robot.


### Assembly

When assembling the camera mount, it should be noted that the lens goes on the
bottom of the mount. When assembled correctly, it is very close to the center
of the pan and tilt servos.


## Problems

Here are a few things to try if the camera is not operating properly.


### Backup Battery

Is the backup battery charged? The camera and it's servos are powered off of
the blue backup battery, not the main battery. This should be the first thing
to check if the camera is not operating properly.


### Wire Connections

Were any wires pulled loose? The camera itself has two PWM cables going into
it. One powers the camera, and is plugged into any free PWM port on the [robot
controller](robot-controller). The other is
plugged into the small TTL/RS-232 converter, which is then plugged into the
[robot controller](robot-controller).


### Status Lights

Are any lights on? The camera itself has three lights. When the camera is in
use, two are lit:

  * A green light in the bottom right of the camera board indicates that the camera itself is receiving power. 
  * A red light in the same place indicates that the camera is locked onto the color it is tracking. 

