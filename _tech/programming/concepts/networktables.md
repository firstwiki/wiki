---
title: NetworkTables
tags: programming
---

{% include stub %}

NetworkTables is a communications protocol used on FIRST robots. It is officially
supported by the WPILib Control Systems team. NetworkTables is used by [GRIP](grip_software),
[SmartDashboard](smartdashboard), and other software to communicate with the 
program running on the robot.

NetworkTables is used to communicate information between several computers. 
There is a single server (often the robot) and zero or more clients. These 
clients can be on the driver station, a coprocessor, or anything else on the
robot's local control network.

As it was intended to only be used on trusted networks, NetworkTables has no
authentication or encryption, and should never be used on untrusted networks
such as the Internet.

## History

NetworkTables was introduced in 2011 as a way for 

NetworkTables v2 was introduced in 2012, and . However,

NetworkTables v3 was introduced in 2015, and the Java/C++ libraries were
completely rewritten.

## Implementations

Official implementations:

* [ntcore](https://github.com/wpilibsuite/ntcore)

Unofficial implementations:

* [C#](https://github.com/robotdotnet/NetworkTables)
* [Node.js](https://github.com/erikuhlmann/ntcore_node)
* [Python](https://github.com/robotpy/pynetworktables)
* [Python + Javascript](https://github.com/robotpy/pynetworktables2js)

