---
title: Electrical Connectors
tags: aux-cs
---

{% include stub %}

Several types of electrical connectors are commonly used in FRC. Some connectors can simply take a bare wire while some require a crimp or solder connection to create a proper electrical connection. Most of these come in several shapes and sizes with different gauges. As always check the manual for the current game to see proper sizing requirements.

## PWM Headers (.1 in)

Commonly used for [PWM Cables](/pwm-cable), these headers have a .1 in pitch and come in various numbers of connectors. The most common is three connector versions, used for [motor controllers](speed-controller) and various other connectors on the [roboRIO](roboRIO), include [analog](analog) and [digital](digital) signals, [relays](spike-relay) and analog inputs. These also come in 2 connector versions, mainly for the robot status light. Four connector and larger versions can also be found on the [roboRIO](roboRIO) for other communications types.

## Weidmuller Connectors

Found on the new [Power Distribution Panel](PDB), [Voltage Regulation Module] and [Pneumatic Control Module], these connectors operate by using a simple button to release the connector inside and allow a bare or tinned wire to be inserted. Some teams prefer to use [Ferrules](http://www.ctr-electronics.com/cabling/ferrule-16-awg.html) instead so that frayed wires do not come out of the connectors. Make sure not to fray the wires beforehand, otherwise the wires themselves may not insert correctly and either may fray out of the connector or the entire wire itself can come out. This type of connector is used on all of the modern [CAN](can) connectors on the entire control system, including the new [roboRIO](roboRIO).

## Wago Connectors

Found on both the new and old [Power Distribution Panel](PDB), these allow various different sizes of wire to be inserted without any prior crimp. Simply by sticking a flat head screwdriver into the opening slots above (or a specific WAGO opening tool if needed), you can insert a wire into it. Unless you have the specific Wago opening tool, it may be hard to open the connectors once inserted into the robot or a enclosure.

## Screw terminals

Commonly found on [motor controllers](speed-controller) for power input and motor output, these connectors require a crimp on the wire end. Once the screw is removed, you can insert the ring crimp above the hole and then insert the screw back in. These screws are easily lost, so if a motor controller dies, make sure to save these for backups. These connectors are not found on [Talon SRXs](talon-srx) or [Victor SPs](victor-sp).

## Spade terminals

Only found on the [Spike Relay](spike-relay), these connectors are also commonly used for wire to wire connectors on the robot.

## Anderson Powerpole

_Not to be confused with Anderson SB-50 connectors_

Powerpoles are commonly used for wire to wire connectors on the robot. They come in 15, 30 and 60 amp varieties. They snap together quite well, can be attached in pairs of two to make sure DC pairs stay together. The two sides of the connector lock together, and teams commonly zip tie the connectors for more secure connections. They also come in many colors, but many teams keep them in pairs of red/black and white/green to match the colors on most [motor controllers](speed-controller). These connectors are hard to crimp without the specific anderson crimping tool, adding additional cost.

## Anderson SB-50

This connector is used for the main battery connector.

## IDC connectors

Used for MXP connectors on the [roboRIO](roboRIO), the sensor mount on the [Talon SRX](talon-srx) and other connectors on the [roboRIO](roborio).

## USB

A USB type B connector is found on the [roboRIO](roborio).

## Barrel jack

Used to power the robot radio.

## RJ45 (ethernet)

Used to connect the [roboRIO](roborio) and robot radio as well as other custom devices on the robot.

## RJ11

Used on the now obsolete [Jaguar motor controller](jaguar) for [CAN](CAN) connections.
