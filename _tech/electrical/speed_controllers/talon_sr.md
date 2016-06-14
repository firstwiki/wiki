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

During a fault the output of the Talon is disabled until the fault condition is no longer present. This fault state is only present on the newer Talon SR, not the older Talon model.

## Programming



## History
