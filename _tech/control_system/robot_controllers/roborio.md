---
title: RoboRIO
tags: robot-controllers
---

{% include stub %}

The roboRIO is a [robot controller](robot-controller) manufactured by National Instruments. It was introduced in 2015 replace the [cRIO](crio)(and subsequent [cRIO II](crio-ii)). It features several types of outputs in inputs, described in the "ports" section of this article.

## Ports

The roboRIO features several types of ports designed for interfacing with various different FIRST regulated devices.

### PWM

There are 10 [PWM](pwm) [cable](pwm_cable) ports along the right side of the roboRIO. These are standard .1 in Pitch, three pin headers, the same as on most [speed controllers](speed-controller). There are three more PWM headers avilable on the MXP header.

### Analog

There are four [analog](analog) in ports on the bottom of the roboRIO. These will take 0 to 5 volt input on the "S" channel, then relay the signal to the processor. These are also standard 0.1 in pitch, three pin headers, with the other two channels being 5v and ground.

There are also two Analog out ports located in the MXP. These are pins 2 and 4, for output 0 and 1 respectively. These can generate 0 to 5 volts each.  

### I2C, SPI, CAN and RS-232.

#### I2C [TODO]

#### SPI [TODO]

#### CAN (or CAN-bus) [TODO]

#### RS-232 [TODO]

### RSL [TODO]

The Robot Status Light (RSL) is a safety feature that allows anyone in the proximity of the robot to know if the robot is enabled or not.

![RSL Wiring](https://alex-spataru.gitbooks.io/frc-robot-programming/content/Images/RSL.jpg)

| Code     | Meaning                                          |
| -------- | -------------------------------------------------|
| Solid On | Robot on and disabled                            |
| Blinking | Robot on and enabled                             |
| Off      | Robot off, roboRIO not powered or bad RSL wiring |

### MXP Port



## Technical



### Status LEDs

There are 6 LEDs located on the top right of the roboRIO to indicate various statuses of the roboRIO and other devices connected to it. Going from top to bottom:

#### Power LED

The power LED has five states, off, green, red solid, red flashing, and yellow. If the LED is off, the voltage is either disconnected or under 4.5 V. If it is green, it is in valid range with no faults. If the status LED is solid red, one of the three voltage rails (6, 5, and 3.3 volts) are short circuiting or are drawing too much current. Check all your wiring to make sure there are no exposed terminals or other extraneous devices that may be drawing too much current from the roboRIO.

If the power LED is flashing red, the input voltage is too high, over 16 V, and all outputs have been disabled. This includes the RSL. If the power LED is solid yellow, one of the brownout conditions have been detected, see the section below on more info on brownouts.

| Color                          | Meaning                                       |
| ------------------------------ | --------------------------------------------- |
| <font color=green>Green</font> | Power is good                                 |
| <font color=amber>Amber</font> | Brownout protection tripped, outputs disabled |
| <font color=red>Red</font>     | Power fault                                   |

#### Status LED

The status LED has five possible states, and is determined by the number of flashes for every few seconds. This LED is off during usual operation, and should only be on when the roboRIO is first booting, either from voltage being applied, or the reset button being pressed. This is commonly known as POST (power-on self test).

If the LED is solid or is continuously flashing without pause, the device is in a unrecoverable error. NI recommends you contact them if this happens. If the status LED flashes twice every few seconds, there is a non fatal error in the software. This is common when you attempt to upgrade the software on the roboRIO and are interrupted. Reinstall the software, using the roboRIO configuration tool, found in the LabView files, to regain the device.

If the LED is flashing three times every few seconds, the device is in safe mode. [TODO: Add Safe Mode info]. If the LED is flashing four times every few seconds, the device software has crashed twice without rebooting or cycling power between crashes. This commonly happens when the roboRIO runs out of memory. Review your code or other applications running on your roboRIO, such as [mjpg-streamer](mjpg-streamer) to solve this issue.

| Code           | Meaning                                 |
| -------------- | --------------------------------------- |
| Two blinks     | Software error                          |
| Three blinks   | Safe mode                               |
| Four blinks    | Sofware crashed twice without rebooting |
| Constant flash | Unrecoverable error                     |
| Solid on       | Unrecoverable error                     |

#### Radio LED

The NI manual states that this status LED is only used for USB attached WiFi radios, as compared to FRC's required external radio, so it's unsure if this one if used or not in standard FRC use. See page 19 on the [NI roboRIO FRC User Manual](http://www.ni.com/pdf/manuals/374474a.pdf#page=19) for these states, in case they are implemented.

#### Comm LED

The communications LED states the current status of the communication with the driver station, as shown also in the [driver station](driver-station). If this LED is off, there is no communication with the driver station. If this LED is solid red, there is no code on the roboRIO. This is also shown as the roboRIO is just loading code for about 30 seconds, as the software loads the new code into memory.

If the LED is flashing red, the robot has been E-Stopped by the driver station. If this happens, all outputs are immediately disconnected, and you must hard reset the roboRIO, either by pressing the reset button, or cycling power to the entire robot, to regain communications. If the LED is green, the driver station has communication and the communication protocol is active. Yellow is listed as "reserved" in the manual.

| Code                                 | Meaning                                      |
| ------------------------------------ | -------------------------------------------- |
| Off                                  | No communication                             |
| <font color=red>Red</font> solid     | Communication with DS, no user code          |
| <font color=green>Green</font> solid | Good communication with DS, user code loaded |
| <font color=red>Red</font> blinking  | Emergency stop                               |

#### Mode LED

The mode LED states what game state the game is currently in, such as [Autonomous Mode](autonomous-mode) or TeleOperated mode. This can also be controlled by the driver station when not connected to the [FMS](FMS) and a full field. A off LED means that the robot is either in the disabled state, or is disconnected from the driver station or FMS. A green LED means the robot is in Autonomous Mode. A yellow LED means the robot is in TeleOperated mode. A red LED means the roboRIO is unsure of what state it's in, or is in test mode.

| Color                            | Meaning            |
| -------------------------------- | ------------------ |
| Off                              | Outputs disabled   |
| <font color=orange>Orange</font> | Autonomous enabled |
| <font color=green>Green</font>   | TeleOP enabled     |
| <font color=red>Red</font>       | Test enabled       |

#### RSL LED

This LED acts exactly like the RSL outputs on the bottom left of the roboRIO, and should be referred to in the RSL section above.

### Brownout



### Accelerometer



### Panel Buttons



## Further Reading
[NI roboRIO FRC User Manual](http://www.ni.com/pdf/manuals/374474a.pdf)

[NI roboRIO Specifications](http://www.ni.com/pdf/manuals/375275a.pdf)

[WPILib Status Light Quick Reference](http://wpilib.screenstepslive.com/s/4485/m/24166/l/144972-status-light-quick-reference)
