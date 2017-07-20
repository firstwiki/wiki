---
title: cRIO
tags: [robot-controllers, obsolete-part]
---

{% include historical %}
{% include outdated-warning %}

The FIRST Robotics Competition (FRC) adopted the CompactRIO (cRIO) control system for advanced robotics for its 2009 through 2014 seasons. In 2010, the cRIO-FRC was joined by the smaller, lighter and cheaper cRIO-FRC II. In 2015, it was replaced by the NI RoboRIO. The cRIO-FRC from National Instruments can be programmed in LabVIEW or C.


##  Programming

Code is cross-compiled on a separate computer then uploaded over the network by the programming environment.


###  LabVIEW

The cRIO was programmable from National Instrument's own environment, LabVIEW. A demonstration of how LabVIEW will be used with the FIRST Robotics Competition robots has been provided by NI [FIRST Robotics Competition: Joystick Motor Control in 10 Minutes](http://zone.ni.com/devzone/cda/tut/p/id/7977 "http://zone.ni.com/devzone/cda/tut/p/id/7977")

###  C++

In addition, the cRIO will be programmable in C or C++ with a library developed by [Worcester Polytechnic Institute](http://first.wpi.edu/"http://first.wpi.edu/") called [WPILib](wpilib). Generated API documentation under very active development (subject to change) can be previewed: [WPI Robotics Library Documentation](http://users.wpi.edu/~bamiller/WPIRoboticsLibrary/index.html "http://users.wpi.edu/~bamiller/WPIRoboticsLibrary/index.html").


###  C

Wrappers around the C++ library will be provided. [[1]](http://forums.usfirst.org/showpost.php?p=18063&postcount=1 "http://forums.usfirst.org/showpost.php?p=18063&postcount=1")


##  Hardware

The Compact Rio contains a PowerPC processor and reprogramable FPGA processor which will be programmed by FIRST for the events. It runs [VxWorks](http://www.wikipedia.org/wiki/VxWorks "wikipedia:VxWorks") [![Image:Extlinkwikipedia.GIF](/media/c/cb/Extlinkwikipedia.GIF)](Image:Extlinkwikipedia.GIF "Image:Extlinkwikipedia.GIF"), a POSIX certified, real-time operating system.


##  Modules

The cRIO has slots for eight interchangeable modules. New modules will be supplied each year to teams. The modules by themselves only have a D-Sub connector, so PWM or other wiring connections are made available through a breakout board that either that screws into the module, or a sidecar that is seperate from the module and connected by a cable.


###  Digital I/O Module (NI 9403) and Sidecar

The Digital Sidecar and module providing general purpose input/output. 32 channels of data are sent to the Digital Sidecar. A digital output can output a maximum of 5.2V.

[Module](http://first.wpi.edu/FRC/digital.html "http://first.wpi.edu/FRC/digital.html")
[Sidecar](http://first.wpi.edu/FRC/digitalsidecar.html "http://first.wpi.edu/FRC/digitalsidecar.html")

###  Digital Output/Solenoid Module (NI 9472) and Solenoid Breakout

The Solenoid module will allow for connections to a pneumatics relay. Connections are provided through the Solenoid Breakout. This module can provide a maximum output of 30V.

[Module and Breakout](http://first.wpi.edu/FRC/solenoid.html "http://first.wpi.edu/FRC/solenoid.html")

###  Analog Input Module (NI 9201) and Analog Breakout

The Analog Input module allows eight inputs of analog data with 12-bit resolution.

[Module and Breakout](http://first.wpi.edu/FRC/analog.html "http://first.wpi.edu/FRC/analog.html")


## Key features

* 32-bit real-time processor 
* 802.11 pre-n wireless ethernet 
* FPGA I/O control 
* Programmable in C, C++, and LabVIEW 
* Wireless debugging 
* Laptop dashboard 
* Intelligent robotics algorithms 
* Real-time vision processing 
* 50G shock rating 
* Easier connectivity 
* More sensor choices 
* More I/O lines 
* Customizable I/O possible in future years 

## External Links

* [FIRST Documentation](http://www.usfirst.org/community/frc/content.aspx?id=10934 "http://www.usfirst.org/community/frc/content.aspx?id=10934")
* [NI FIRST community](http://decibel.ni.com/content/community/first "http://decibel.ni.com/content/community/first")
* [WPIlib resources, C and C++ programming](http://first.wpi.edu/FRC/ "http://first.wpi.edu/FRC/")
