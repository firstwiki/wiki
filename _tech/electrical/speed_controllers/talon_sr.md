---
title: Talon SR
tags: speed-controller
---

{% include stub %}

## Technical

The Talon SR is a legal FIRST [Speed Controller](speed-controller) to use in the FIRST Robotics Competition. It recieves a [PWM Signal](pwn-signal) from the [roboRIO](roborio) or other [robot controller](robot-controller).

### Use

To connect, attach a [PWN cable](pwm-cable) to the PWM port on the Talon and two input wires, 12V and ground, from the [PDB](PDB), and -12v and +12v to the [motor](motors). The PWM cable is tight, this is a feature to keep PWM cables from falling out during matches. To insert, make sure the PWM Cable is straight and a 90 degree angle to the controller and push straight into the three pin port. It's common to catch on the side of the shroud and bend the pins. If this happens, take out the PWM cable, straighten the pins as best as you can, replace the cable if it's un reparable, and attempt again. The polarity **does** matter, and the black cable (or brown) should be near the embossed "B" on the surface. While color doesn't matter in the usual sense, conforming to standards of ground color is useful, especially when debugging or in inspection.

To insert the motor and input voltages, unscrew the retaining screw, and place your #6 crimps include in the [Kit of Parts](kit-of-parts) inside the contact area. Line up the bolt, and screw it in. The positive terminal on the intake voltage side is labeled with a red "+". The terminal next to it next to the PWM port is the ground connection. Take both these leads to the [PDP](PDP). The opposite side features the motor connections. The terminal closest to the white "M+" figure is the positive motor terminal. This a red wire on [CIM Motors](cim-motor) and [BAG Motors](bag-motor), and a positive terminal on all other motors.

### Coast/Brake

A small jumper on the Talon SR determines whether the Talon will 'coast' or 'brake' when it stops receiving signal. In 'coast' mode, momentum of the spinning motor will enable the motor to coast to a stop when it stops receiving signal. In 'brake' mode, the Talon will short the output terminals together, providing a resistance to the momentum of the spinning motor. As such, the motor will come to a stop much more quickly.

Typically, a robot will use 'coast' mode on most drive motors, as abrupt stops can cause tipping issues. Turrets, arms, and other manipulators should usually use 'brake' mode, both to help hold a load at its desired position and to aid in controllability.

### LED Status

The Status LED, located next to the break/coast jumper, and the calibration button, can show the user a variety of useful debugging statuses. The LED states during calibration are in the calibration section. The Status LED can be one of three colors: red, orange or green. When not receiving a PWM signal, this LED blinks orange. This could be because the PWM Cable is not connected, or in FRC, the robot is in the disabled state.

When receiving a PWM signal, the LED will blink according to what speed the signal is telling it. If it's at a full stop, or with the 4% dead band on the Talon, the LED will be solid orange. If it's being told to go forward, the LED will blink green. The faster the LED blinks, the faster the signal is telling it to go. A solid green LED means it's receiving 100% throttle forward. A solid red LED is 100% backwards.

Another LED is state is the fault state. This is when the Talon blinks it's LED between red and orange. A fault can be caused by one of three things:

* Under voltage (< 3.3V DC)
* Over temperature (>170 degrees C)
* A shorted output transistor.

During a fault the output of the Talon is disabled until the fault condition is no longer present. This fault state is only present on the newer Talon SR, not the older Talon model. The last LED state is flashing red/green, which is enabled during calibration.

### Calibration

You can calibrate the Talon if the controller isn't properly responding to PWM inputs. Do the following if any of the following symptoms are occurring:

* Neutral on joystick not stopping the motor (solid yellow LED)
* Full throttle on joystick not doing the same on controller (Not solid LEDs when maxed on joystick)
* Maxing out throttle on controller (solid LED) before joystick fully maxed.

The calibration process will reset the maximum, minimum, and middle PWM values. Follow the follow steps to calibrate your Talon:

1. Using a paper clip or other small pointed stick, press and hold the red button near the label "CAL". The LED should begin to flash red/green, meaning you've enabled calibration mode.
2. Keeping the CAL button pressed down, move your joystick or other input device to the maximum and minimum input. Do this as many times that you think you need to fully get the maximum and minimum fully.
3. Move the joystick back to it's center position on the axis that controls the Talon, and release the CAL button.
4. If successful, the LED will blink green several times. The calibration may fail, resulting in the flashing on the LED red several times. In this case, the Talon will used the last valid calibration values.

Calibration values are stored in memory after power cycles or resets, and the defaults are set for most standard FRC compatible joysticks.


## Programming

### Creating a Talon object

To create an instance of a Talon Sr, use the [Talon class](http://first.wpi.edu/FRC/roborio/release/docs/java/edu/wpi/first/wpilibj/Talon.html):
```java
import edu.wpi.first.wpilibj.Talon; //Import Talon
//...
Talon t = new Talon(0);
```
The above example will create a Talon object named `t` connected to PWM channel 0.

### Setting a Talon's motor speed

To set a Talon's motor speed, use the [`set()`](http://first.wpi.edu/FRC/roborio/release/docs/java/edu/wpi/first/wpilibj/Talon.html#set-double-) method:
```
Talon t = new Talon(0); //See previous section
t.set(1.0); //Sets the Talon to max speed
```
The speed of the Talon is from -1.0 to 1.0.
1.0 is full speed forward, and -1.0 is full speed backward.

## History

The Talon was originally introduced for the 2013 season in mid 2012 for off-season testing and beta team testing. They were made legal in the 2013 season. After the 2013 season, CTR electronics, the manufacturers, noticed a few issues and decided to fix these in a new, updated, motor controller called the Talon SR. There were very few changes to this new model. One of them was the introduction of Synchronous sign magnitude rectification. This is a change that doesn't change much in the driving style of the Talon, but should make it run colder. The LED status lights were also changed slightly. In 2015, they were discontinued for the advent on the new [Talon SRX](talon-srx). As of the 2016 season, they are still legal motor controllers. 
