---
title: cRIO-FRC
tags: [robot-controllers, control-system, obsolete-part]
---

{% include historical %}

The FIRST Robotics Competition (FRC) adopted the CompactRIO (cRIO) control system for advanced robotics for its 2009 through 2014 seasons. In 2010, the cRIO-FRC was joined by the smaller, lighter and cheaper cRIO-FRC II. In 2015, it was replaced by the NI RoboRIO. The cRIO-FRC from National Instruments can be programmed in LabVIEW, C++ or C.


##  Programming

Code is cross-compiled on a separate computer then uploaded over the network by the programming environment.


###  LabVIEW

The cRIO was programmable from National Instrument's own environment, LabVIEW. A demonstration of how LabVIEW will be used with the FIRST Robotics Competition robots was provided by NI (link not found).

###  C++

In addition, the cRIO was be programmable in C or C++ with a library developed by [Worcester Polytechnic Institute](https://web.archive.org/web/20170509210113/http://first.wpi.edu/ "https://web.archive.org/web/20170509210113/http://first.wpi.edu/") called [WPILib](wpilib). API documentation generated during active development can be viewed: [WPI Robotics Library Documentation (2009)](https://web.archive.org/web/20170111233254/http://users.wpi.edu/~bamiller/WPIRoboticsLibrary/index.html "https://web.archive.org/web/20170111233254/http://users.wpi.edu/~bamiller/WPIRoboticsLibrary/index.html").


###  C

Wrappers around the C++ library were provided. [[1]](http://web.archive.org/web/20170720203728/https://forums.usfirst.org/forum/general-discussions/first-programs/first-robotics-competition/competition-discussion/programming-aa/c-c-ac/4278-wpi-robotics-library-c-c-edition-documentation?postcount=1 "http://web.archive.org/web/20170720203728/https://forums.usfirst.org/forum/general-discussions/first-programs/first-robotics-competition/competition-discussion/programming-aa/c-c-ac/4278-wpi-robotics-library-c-c-edition-documentation?postcount=1")


##  Hardware

The Compact Rio contains a PowerPC processor and reprogramable FPGA processor which was programmed by FIRST for the events. It ran [VxWorks](http://www.wikipedia.org/wiki/VxWorks "wikipedia:VxWorks"), a POSIX certified, real-time operating system.


##  Modules

The cRIO had slots for eight interchangeable modules. New modules were supplied each year to teams. The modules by themselves only have a D-Sub connector, so PWM or other wiring connections are made available through a breakout board that either that screws into the module, or a sidecar that is seperate from the module and connected by a cable.


###  Digital I/O Module (NI 9403) and Sidecar

The Digital Sidecar and module provide general purpose input/output. 32 channels of data are sent to the Digital Sidecar. A digital output can output a maximum of 5.2V.

[Module](https://web.archive.org/web/20170720195845/http://first.wpi.edu/FRC/digital.html "https://web.archive.org/web/20170720195845/http://first.wpi.edu/FRC/digital.html")  
[Sidecar](https://web.archive.org/web/20170720201529/http://first.wpi.edu/FRC/digitalsidecar.html "https://web.archive.org/web/20170720201529/http://first.wpi.edu/FRC/digitalsidecar.html")

###  Digital Output/Solenoid Module (NI 9472) and Solenoid Breakout

The Solenoid module will allow for connections to a pneumatics relay. Connections are provided through the Solenoid Breakout. This module can provide a maximum output of 30V.

[Module and Breakout](https://web.archive.org/web/20170720201939/http://first.wpi.edu/FRC/solenoid.html "https://web.archive.org/web/20170720201939/http://first.wpi.edu/FRC/solenoid.html")

###  Analog Input Module (NI 9201) and Analog Breakout

The Analog Input module allows eight inputs of analog data with 12-bit resolution.

[Module and Breakout](https://web.archive.org/web/20170720202106/http://first.wpi.edu/FRC/analog.html "https://web.archive.org/web/20170720202106/http://first.wpi.edu/FRC/analog.html")


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

## External Links

* [WPIlib resources, C and C++ programming](https://web.archive.org/web/20170115115408/http://first.wpi.edu/FRC/index.html "https://web.archive.org/web/20170115115408/http://first.wpi.edu/FRC/index.html") (2010)
* [WPIlib ScreenSteps Documentation](https://web.archive.org/web/20170301213604/http://wpilib.screenstepslive.com/s/3120 "https://web.archive.org/web/20170301213604/http://wpilib.screenstepslive.com/s/3120") (2014)
